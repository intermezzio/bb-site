---
title: 'Sprint 3 and Beyond'
date: 2018-11-18T12:33:46+10:00
draft: false
weight: 3
heroHeading: 'Integrating all features into one product'
heroSubHeading: 'Improve the chassis, integrate new motors, and send joystick commands'
heroBackground: 'work/work1.jpg'
thumbnail: 'work/work1-thumbnail.jpg'
images: ['https://source.unsplash.com/random/400x600/?nature', 
'https://source.unsplash.com/random/400x300/?travel','https://source.unsplash.com/random/400x300/?architecture','https://source.unsplash.com/random/400x600/?buildings','https://source.unsplash.com/random/400x300/?city','https://source.unsplash.com/random/400x600/?business']
---

## Sprint Goal
Our goal for this sprint was to integrate the wireless drive code with the newly built, three-wheel chassis.

## Subteam Progress
### Software
Our goal for the final sprint was to update the firmware to drive with three wheels instead of two, and to make the controller more intuitive by creating a virtual joystick controller that would send commands to the robot. The joystick sends angle and magnitude information, which is converted to wheel speeds in a Python script in order to reduce the amount of computation that the Arduino does. The wheel speeds are parsed by the Arduino and the motors respond accordingly.

### Mechanical
In this sprint, we focused on making our robot drive better.  We finally received our omni wheels in the mail and realized they had a much harder time trying to overcome the bumps in the ball compared to the larger wheels we were using before.  We tried a few different things, but turns out the best way to make the ridges in the ball more approachable is to duct tape pipe cleaners to either side of the bumps.  This makes the lip up to the ridge much smoother and more like a ramp than a curb.  We also created a protective dome to house our electronics.

### Electrical