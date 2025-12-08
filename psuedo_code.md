🧪 1. Gas Leakage Detection (Arduino + MQ-6 + GSM)

start

initialize mq6_sensor
initialize led
initialize buzzer
initialize gsm_module

loop forever:
    read analog_value from mq6_sensor
    ppm = convert_to_ppm(analog_value)

    if ppm >= low_threshold and ppm < high_threshold:
        turn_on(led)
        send_sms("Warning: LPG leak detected (Low Level)")

    else if ppm >= high_threshold:
        turn_on(led)
        turn_on(buzzer)
        send_sms("ALERT! Dangerous LPG leak detected!")

    else:
        turn_off(led)
        turn_off(buzzer)

    delay(1000 ms)
end loop


2. Weight Monitoring (Load Cell + HX711 + Arduino Uno)

initialize HX711
initialize LCD

tare = read_load_cell()

scale_factor = calibrate_with_known_weight()

loop forever:
    raw = read_load_cell()
    weight = (raw - tare) / scale_factor

    display weight on LCD

    if weight < refill_limit:
        display "Refill Soon" on LCD

    if weight < empty_limit:
        display "Cylinder Empty"

    delay(1000 ms)
end loop



📱 3. Android App → Arduino Communication

via Bluetooth 

if data_received_from_app:
    parse_command()

    if command == "STATUS":
        send current_weight + gas_level back to app

    if command == "TEST_ALARM":
        activate buzzer and led



📲 4. GSM SMS Logic

function send_sms(message):
    gsm_module.send("AT+CMGF=1")        // SMS mode
    gsm_module.send("AT+CMGS=\"+91XXXXXXXXXX\"")
    gsm_module.send(message)
    gsm_module.send(CTRL+Z)            // send message
