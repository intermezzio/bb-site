---
title: 'Firmware'
date: 2018-11-28T15:15:26+10:00
icon: 'icons8-arduino-100.png'
draft: false
featured: true
weight: 4
heroHeading: 'Firmware'
heroSubHeading: 'How the robot is programmed to operate'
heroBackground: 'services/service1.jpg'
---

The Arduino's firmware is all written in Arduino C and allows BB-8 to receive
commands from a laptop and output speeds to its motors. The firmware is short
and to the point, as firmware should be.

## Code Summary

The code starts by setting all of the speeds to zero. When a bluetooth signal
is received, it parses the command, which gives it three numbers: the signed
percentage power values for the three motors. These values are normalized and
the motors are then set to run at the relative speeds they were assigned.
The firmware keeps doing this continuously, _unless there is no command sent for
30 seconds, in which case the motors are stopped_. This failsafe is included
in case electrical components stop working during a run and the motors need to stop
running but the bluetooth connection fails.

## Libraries Used

1. **\<Adafruit_MotorShield.h>** is used for interfacing the Motor Shield. See
	more information in the electrical section.
2. **\<SoftwareSerial.h>** is used for feeding bluetooth commands to the Arduino
	via a non-default port.

## More Information

The firmware for the Arduino, along with the rest of the software, can be found
on [GitHub](https://github.com/intermezzio/bb-8).