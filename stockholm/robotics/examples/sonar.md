[❮ Back to examples](#!robotics/code-examples.md)
# Sonar

## Overview
Example of how to use a Sonar sensor to measure distance.

## Material
* 01 x Sonar
* 01 x Arduino
* 03 x Female-male jumper wires

## Circuit
![](https://cloud.githubusercontent.com/assets/122277/4790890/d04e698a-5dd6-11e4-8b60-76fe0996179a.png)


## Instructions
#### 1. Connect the 3 male-female wires from the Arduino to the Sonar.

* The negative wire (recommended color: black) goes from ```GND``` on the Arduino to ```Gnd``` on the Sonar.
* The positive wire (recommended color: red) goes to from ```5V``` on the Arduino to ```Vcc``` on the Sonar.
* The control wire (recommended color: anything but red or black) goes from pin ```7``` on the Arduino, to both ```Echo``` and ```Trigger``` on the Sonar. You need need to bend the Sonar pins a little bit and force the jumper wire in. If you need any help please ask one of the facilitators.

(TODO: add picture of how to connect wires to the Sonar) 

#### 2. Open the Serial Monitor
After you program your board, open the Serial Monitor and  watch the Sonar values appear on the screen.

##Code
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/sketch:57083" frameborder="0"></iframe>
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/serialmonitor" frameborder="0"></iframe>

##Exercise
1. How do you think the Sonar works? A tip: it's the same technique bats use to "see in the dark".
2. How far can the Sonar "see"? Stay in front if the Sonar and move back slowly and see if the values change.
