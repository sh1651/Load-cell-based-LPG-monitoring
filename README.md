**IoT-Based Gas Monitoring**
IoT-enabled smart gas monitoring system that detects gas leakage, tracks cylinder weight in real-time, and sends instant alerts to users through a mobile application

**Project Objective**
- Monitor gas leakage and instantly alert the customer
- Help the customer know when to replace the cylinder
- Provide continuous gas level updates 

**Solution**

  NodeMCU (esp8266) based Iot device uses Load cell to calculate the amount of gas left
  and give the info in the app and also on the display and a added security feauture to check and 	alert the user in case of a leak gas leak

**Hardware used** 
	NodeMCU
	Load Cell
	HX711 Amplifier
	MQ-6 Sensor
	16×2 LCD
	Buzzer
	
<img width="1191" height="607" alt="image" src="https://github.com/user-attachments/assets/7a13163c-a660-4592-9852-73e59125d3ac" />
**Software Used**
Arduino IDE

libraries used

- ESP8266WiFi.h 
- HX711.h 
- LiquidCrystal_I2C.h 

**Circuit building**
stage 1:
<img width="992" height="645" alt="image" src="https://github.com/user-attachments/assets/45cee7a8-9af2-413d-b77f-49abd19ad1d5" />

final stage :
<img width="496" height="660" alt="image" src="https://github.com/user-attachments/assets/b401e95d-5339-4b09-887c-49f86f014d99" />

**Results**

- LPG detection working
- Load cell successfully calibrated
- Real-time LCD display
- Fully functional prototype
 
 **Limitations**
 
- Weight data affected by vibrations
- Needs stable mounting
- Internet required for IoT features

**Team**
  This project was developed as a team effort during the COVID-19 pandemic.
Hardware design and assembly
Software development
Testing and calibration
Documentation

**My Experiecne**

This was my first team-based project, which taught me valuable lessons in:
Team Management: Coordinating tasks and deadlines effectively
Skill Assessment: Identifying each member's strengths and delegating accordingly
Problem Solving: Overcoming COVID-19 limitations
Resource Management: Working within budget constraints
Technical Skills: Hands-on experience with IoT, sensors, and microcontrollers

Despite challenges like the inability to manufacture a custom PCB due to budget and pandemic restrictions, we successfully delivered a functional prototype that meets all core objectives. -
