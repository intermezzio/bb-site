---
title: 'Electrical'
date: 2018-11-18T12:33:46+10:00
icon: 'icons8-circuit-100.png'
draft: false
featured: true
weight: 1
heroHeading: 'Electrical'
heroSubHeading: 'How BB-8 is powered and controlled'
heroBackground: 'gallery/sprint2/chassis_top.jpg'
---

An Arduino controls all of the electrical components on BB-8. The Arduino is connected
to various other components, including motors and a bluetooth module, to drive BB-8.

## Circuit Design
Here is the layout of our circuit:

![image](../../images/circuit_diagram.png)

The circuit includes an Arduino, a motor shield, and an HC-05 bluetooth chip.
The bluetooth module pairs with a laptop and connects to the Arduino to send
and receive commands. The motor shield sends power to the motors to drive them.

## Parts Used
- Arduino Uno
- Adafruit Motor Shield v2
- HC-05 Bluetooth Chip (chip that recieves bluetooth sinal and sends it to the arduino over serial.)
- 3 x 18650 Batteries (Run in series for a total of 12V)