---
title: A first look at the raspberry Pi Pico
description: Alter your site config
date: 2021-06-20
tags:
  - posts
layout: layouts/post.njk
---

[<img src="https://cdn-images-1.medium.com/max/1600/0*cAnqBUCAB5amHM0u" width="650"/>](image.png)

## What is the pico?
The pico is a new microcontroller from the raspberry pi foundation. The pico uses a custom ASIC chip designed by the raspberry pi foundation specifically for the raspberry pi pico. The chip is called the RP2040 the RP2040 is based off of the Arm Cortex M0+ processor. The RP2040 has 2 cores at 133 MHz.
## What can I use the pico for?
You can use the pico instead of any other microcontroller in any of your projects. As the pico is only $4! And has considerably higher performance than the Arduino and most other microcontrollers though the pico is harder to get started with because you have to solder on the pin headers and it has less integration with the Arduino build environment. On the other hand the pico also has plenty of IO for all of your needs with 2 × SPI, 2 × I2C, 2 × UART, 3 × 12-bit ADC, 16 × controllable PWM channels. And 26 multi-function GPIO pins. Overall the pico is a great in between choice if you are looking for something with performance in between an Arduino nano and a teensy 4.0.
## What is the performance like on the pico?
The pico has 2 cores at 133 MHz. Which is considerably more powerful than any Arduino. Also since the RP2040 has 2 cores you can do multithreading on the raspberry pi pico for even better performance. The pico has enough performance for almost any project you have. Also most microcontrollers have to bit bang which takes additional processing power. But the raspberry pi pico has 8 × Programmable I/O (PIO) state machines. Which means it can control IO without having to bit bang. Though the performance benefits of not having to bit bang depend on the I/O you will be using.