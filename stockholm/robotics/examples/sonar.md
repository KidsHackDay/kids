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
Connect the 3 wires to the Sonar, the negative wire (recommended color: black) goes to ```Gnd```, the positive wire goes to ```Vcc``` (recommended color: red).

The control wire (recommended color: anything but red or black) needs to connect to both ```Echo``` and ```Trigger```. You need need to bend the Sonar pins a little bit and force the jumper wire in. If you need any help please ask one of the facilitators.

TODO: add picture of how to connect wires

After you program your board, open the Serial Monitor and see watch the Sonar values on the screen.

##Code
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/sketch:57083" frameborder="0"></iframe>

## Serial Monitor
<iframe style="height: 510px; width: 100%; margin: 10px 0 10px;" allowTransparency="true" src="https://codebender.cc/embed/serialmonitor" frameborder="0"></iframe>

##Exercise
1. How far can the Sonar "see"? Try to point the Sonar to different obejcts.
2. How do you think the Sonar works?
