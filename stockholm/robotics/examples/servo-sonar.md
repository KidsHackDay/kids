[❮ Back to examples](#!robotics/code-examples.md)
# Sonar controlled by Sonar

## Overview
Example of how to use a Sonar sensor to control the movements of a Servo Motor

## Material
* 01 x Sonar
* 01 x Servo
* 01 x Arduino
* 03 x Female-male jumper wires
* 03 x Male-male jumper wires

## Circuit
![](https://cloud.githubusercontent.com/assets/122277/4791249/fb961cb0-5dda-11e4-835f-6ae57954251d.png)


## Instructions
1. Connect the 3 male-female wires from the Arduino to the Sonar.
  1.1. The negative wire (recommended color: black) goes from ```GND`` on the Arduino to ```Gnd``` on the Sonar.
  1.2. The positive wire (recommended color: red) goes to from ```5V``` on the Arduino to ```Vcc``` on the Sonar.
  1.3. The control wire (recommended color: anything but red or black) goes from pin ```7``` on the Arduino, to both ```Echo``` and ```Trigger``` on the Sonar. You need need to bend the Sonar pins a little bit and force the jumper wire in. If you need any help please ask one of the facilitators.

TODO: add picture of how to connect wires

Connect the wires male-male wires from the Arduino to the Servo.
* The negative wire goes from ```GND``` on the Arduino to the ```black/brown wire``` on the Servo.
* The positive wire goes from ```5V``` on the Arduino to the ```red wire``` on the Servo.
* The control wire goes from pin ```8``` on the Arduino to the ```yellow wire``` on the Servo.

Run the code!

##Code
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/sketch:57083" frameborder="0"></iframe>
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/serialmonitor" frameborder="0"></iframe>

##Exercise
1. Can you use the servo to move something from far away?
2. How fast can the servo move?
