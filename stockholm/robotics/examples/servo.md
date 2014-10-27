[❮ Back to examples](#!robotics/code-examples.md)
#Servo

## Overview
Example of how to control a servo.

## Material
* 01 x Servo
* 01 x Arduino
* 03 x Male-male jumper wires

##Circuit
![](https://cloud.githubusercontent.com/assets/122277/4790256/02d2fdc4-5dcf-11e4-9bd0-84f77636d92b.png)

## Instructions
#### 1. Connect the wires male-male wires from the Arduino to the Servo.

* The negative wire goes from ```GND``` on the Arduino to the ```black/brown wire``` on the Servo.
* The positive wire goes from ```5V``` on the Arduino to the ```red wire``` on the Servo.
* The control wire goes from pin ```8``` on the Arduino to the ```yellow wire``` on the Servo.

##Code
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/sketch:55971" frameborder="0"></iframe>

##Exercise
1. Change the ````wave.duration```` to different numbers. If you use a small number, will the movement be slower or faster?
2. Can you add a Led to your circuit and make it blink in the same speed as the servo?
