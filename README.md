#  Brushless Dc Motor
A BLDC motor consist of two main parts, a stator and a rotor. The rotor is a permanent magnet with two poles, while the stator consists of coils arranged. If we apply current through a coil it will generate a magnetic field and the magnetic field lines or the poles depends on the current direction, so if we apply the appropriate current, the coil will generate a magnetic field that will attract the rotors permanent magnet. Now if we activate each coil one after another the rotor will keep rotating because of the force interaction between permanent and the electromagnet. In order to increase the efficiency of the motor we can wind two opposite coils as a single coil in way that will generate opposite poles to the rotor’s poles, thus we will get double attraction force.
## Electronic Speed Control
in order the rotor to make full cycle we just need to activate the correct two MOSFETS in each of the 6 interval and that’s what (ESC) are all about. An electronic speed control (ESC) is an electronic circuit that controls and regulates the speed of an electric motor. It may also provide reversing of the motor and dynamic braking. Miniature electronic speed controls are used in electrically powered radio-controlled models.
## List of Components
1.	Arduino UNO
2.	BLDC outrunner motor (Any other outrunner motor will work fine)
3.	Electronic Speed Controller (Choose according to the current rating of the motor)
4.	LiPo Battery (to power the motor)
5.	Male-Male Jumper cable * 3
6.	USB 2.0 cable type A/B (To upload the program and power the Arduino).
## Connections
Connect the motor to the output of ESC. Here, the polarity doesn't matter. If you switch any 2 of the 3 wires, the motor will rotate in opposite direction. Connect the '+' & '-' of battery to the Red (+) and Black (-) wires of ESC respectively. From the 3pin servo cable coming out of the ESC, connect the Brown cable to the 'GND' pin on Arduino. Connect the Yellow cable to any digital pin. In our case its digital pin 12.
Programming Arduino UNO
Connect the Arduino to the PC. Open Arduino IDE and write this code. Under 'Tools' select Board: Arduino/Genuino UNO Port: COM15 (Select appropriate COM port. To find out the COM port open device manager and look for Arduino UNO under 'Ports'). Click Upload button on the upper left corner.

![BLDC](https://user-images.githubusercontent.com/109004035/178165599-2f852d0d-7888-4647-ae89-bb3f815e9574.jpeg)


## Run The Motors
1. Connect the battery to the ESC to power up the ESC.
2. Power the Arduino.

**If you do the other way round, the Arduino will run the arm sequence and the ESC will miss those commands since it isn't powered up. In this case press the reset button on the Arduino.**

