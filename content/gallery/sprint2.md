---
title: 'Sprint 2'
date: 2018-11-18T12:33:46+10:00
draft: false
weight: 2
heroHeading: 'Modified ball design'
heroSubHeading: 'Improve the chassis and send bluetooth signals'
heroBackground: 'https://source.unsplash.com/iqGtaQnk3VM/1600x400'
thumbnail: 'gallery/sprint2/chassis_bottom.jpg'
images: ['gallery/sprint2/chassis_bottom.jpg', 
'gallery/sprint2/chassis_on_ground.jpg','gallery/sprint2/chassis_top.jpg','gallery/sprint2/hamster_ball.jpg','gallery/sprint2/bluetooth_session.png']
---

In this sprint, we wanted to make our robot wireless.  This included incorporating our Bluetooth module and adding batteries.

## Subteam Progress
### Software
Our goal for this sprint was to incorporate the HC-05 bluetooth module onto the robot chassis in order to communicate wirelessly with the Arduino and sent commands in real-time. Our approach was to write a Python script that converted keyboard presses into commands that were sent over Serial to the Bluetooth module. The Arduino firmware processed the incoming command and reacted accordingly. Future steps include incorporating some sort of controller, such as a joystick, and updating the Arduino control code to account for three wheels.

### Mechanical
In this sprint, we wanted to address a lot of the issues we were facing last sprint and prepare for our new parts coming in the mail.  We started by trying to add weights to the bottom of our robot to lower the center of gravity.  We then designed and began fabricating our motor and Arduino mounts.  We redesigned our chassis to be 2" smaller and integrate our new motors, batteries, & circuitry.  We assembled our updated chassis with new components.

### Electrical
In this sprint, we built the first battery powered model. This model uses 4 18650 batteries (green on the bottom of the chassis) to power all electrical components on the robot. All components were wired up to the modified chassis and configured to balance the center of gravity of the chassis.
