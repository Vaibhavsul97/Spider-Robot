Legs_int: This file is for servo calibration.
Spider_Main: This is the main code that includes all the movements of the spider robot.


🕷️ Spider Robot
The Spider Robot is a 12-servo quadruped robot controlled via an Arduino UNO. This project includes servo calibration, movement coding, and a customizable control structure, allowing you to create walking, rotating, or advanced motion patterns.

🧩 Hardware Components
Component	Description	Qty
3D Printed Spider Robot Body Kit	Includes body and legs	1
Arduino UNO	Main controller board	1
Arduino UNO USB Cable	For programming the Arduino	1
UNO Experimental Shield	For easy prototyping and servo connections	1
360° Servo Motors	For leg movements (continuous rotation)	12
18650 Battery Holder	Power supply via Li-ion batteries	1
DPDT Self-lock Push Switch	For control input	1
M3 x 30mm Bolts	For assembly	6

🛠️ Servo Pin Configuration
Servos are connected to the Arduino through the UNO Experimental Shield. Set the robot in a neutral "standing" position before calibration.

💻 Software Setup
1. Install Required Libraries
Servo Library (usually pre-installed)
FlexiTimer2 Library (for advanced servo timing)

2. Uploading Code
Open Arduino IDE
Paste the Servo Calibration Code and Main Code
Select board: Arduino UNO
Choose correct COM port
Upload and observe servo initialization

⚙️ Operating the Spider Robot
🔌 Powering
Connect Arduino to USB or external 5V
Power servos via battery holder (ensure sufficient current)

🎯 Calibration
Upload the Servo Calibration Code
All servos move to 90° (neutral/start position)

🕹️ Movement Control

Upload the Main Code to control movements
Customize angles and sequences to create walking, turning, or special actions
servo[0][0].write(30);   // Front-left leg, joint 1
servo[0][1].write(90);   // Front-left leg, joint 2 (neutral)
servo[0][2].write(150);  // Front-left leg, joint 3

🧪 Troubleshooting
Issue	Possible Cause & Fix
Servos not responding	Check wiring and power supply
Code not uploading	Ensure USB connection, correct board & port in IDE
Erratic servo movement	Check for overloaded power or signal wiring interference

🔧 Advanced Control
For complex motion, implement timed loops and gait algorithms. Combine servo angles with delay/timing functions to simulate realistic walking.

✅ Conclusion
The Spider Robot is a great platform for exploring robotics with Arduino. With 12 independently controlled servos and full calibration support, you can expand its movement capabilities, explore walking patterns, and build your own quadruped logic.
