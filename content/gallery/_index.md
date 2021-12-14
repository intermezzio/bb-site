---
title: 'Gallery'
date: 2018-02-10T11:52:18+07:00
heroHeading: 'Gallery'
heroSubHeading: 'How we made BB-8'
heroBackground: 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimages.wired.it%2Fwp-content%2Fuploads%2F2017%2F10%2F10121331%2F1507623211_bb8.jpg&f=1&nofb=1'
---

This BB-8 robot design integrates mechanical, electrical, firmware, and software components
to create a fully navigatable spherical robot. This robot can be controlled via a virtual
joystick, and commands are sent from the joystick to the robot in real time for navigating
in 2D.

![image](../images/Electronics_Flowchart.png) 

On our laptop we convert commands from the joystick into speeds that our three motors should be going. We then send those speeds to the Arduino over bluetooth using the HC-05 blueetooth module to recieve the signal. Then the arduino normalizes the motor speeds and relays the commands to the motor shield to guide the robot in the right direction. 
