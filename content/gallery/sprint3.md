---
title: 'Sprint 3 and Beyond'
date: 2018-11-18T12:33:46+10:00
draft: false
weight: 3
heroHeading: 'Integrating all features into one product'
heroSubHeading: 'Improve the chassis, integrate new motors, and send joystick commands'
heroBackground: 'gallery/sprint3/dome1.jpg'
thumbnail: 'gallery/sprint3/dome1.jpg'
images: ['gallery/sprint3/full_ball.jpg','gallery/sprint3/chassisAngle.png','gallery/sprint3/dome3.jpg','gallery/sprint3/epoxy.JPG','gallery/sprint3/top_chassis.jpg','gallery/sprint3/halves.jpg','gallery/sprint3/chassisTOP.PNG','gallery/sprint3/chassisBottom.PNG']
---

Our goal for this sprint was to integrate the wireless drive code with the newly built, three-wheel chassis, as well as fully integrate all mechanical and electrical components.

## Subteam Progress
### Software
Our goal for the final sprint was to update the firmware to drive with three wheels instead of two, and to make the controller more intuitive by creating a virtual joystick controller that would send commands to the robot. The joystick sends angle and magnitude information, which is converted to wheel speeds in a Python script in order to reduce the amount of computation that the Arduino does. The wheel speeds are parsed by the Arduino and the motors respond accordingly.

### Mechanical
In this sprint, we focused on making our robot drive better.  We finally received our omni wheels in the mail and realized they had a much harder time trying to overcome the bumps in the ball compared to the larger wheels we were using before.  We tried a few different things, but turns out the best way to make the ridges in the ball more approachable is to duct tape pipe cleaners to either side of the bumps.  This makes the lip up to the ridge much smoother and more like a ramp than a curb.  We also created a protective dome to house our electronics.

### Electrical
In this sprint, we determined that the batteries were sending a higher voltage as one test led to the motor shield catching fire. The chassis now runs on 3 batteries instead of 4 and the broken components were replaced. Additionally, we created a dome that protects the electrical components inside of the ball in case the components flip upside down or otherwise experience unexpected forces.