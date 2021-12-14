---
title: 'Software'
date: 2018-11-28T15:15:34+10:00
icon: 'icons8-code-100.png'
draft: false
featured: true
weight: 3
heroHeading: 'Software Design'
heroSubHeading: 'How the server assists in BB-8s Navigation'
heroBackground: 'bb8-in-ship.jpg'
---

The software, written in Python, creates a clean interface for sending commands
to BB-8, converting a joystick input to BB-8 commands.

## Joystick

The joystick is written in HTML/JS using a canvas element. Since this code is
very generic and not central to BB-8's functionality, the frontend of this was
based off of [an existing HTML joystick](https://www.instructables.com/Making-a-Joystick-With-HTML-pure-JavaScript/).
This code was modified to send the position of the joystick (indicating magnitude
and direction) to a Python server.

A Python server works as a REST API for sending joystick commands. The server hosts
a port on localhost and waits for post requests to its address. This request contains
a string to send to the Arduino, which is handled by the bluetooth code.

## Bluetooth

BB-8 has a HC-05 bluetooth module that can pair to most electronic devices. When
this connection is made, a session with the bluetooth module can send data via a
data stream, represented by a filename on Linux and Windows devices. It acts
very similar to the file address of a USB port or other output device. The Pyserial
library can send data to this address and the data is transmitted to the bluetooth
device as if the address were the address of an Arduino, which makes the bluetooth
code very similar to normal serial code. When the Bluetooth module receives messages,
they are all forwarded to the Arduino Sofware Serial port. Initializing this session
can be tricky, but going into advanced device settings on Windows or using `rfcomm`
in Linux can create identical bluetooth sessions, allowing the same code to be run cross
platform.

## Library Used

1. **Pyserial** is used for sending bluetooth commands.

The code did not use any other libraries that aren't builtins, even for the server,
so this is the only software dependency.

## More Information

The software for this project can be found
on [GitHub](https://github.com/intermezzio/bb-8).