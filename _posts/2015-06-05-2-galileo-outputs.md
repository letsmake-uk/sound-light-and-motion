---
layout: handout
title: Outputs
---

<br>

The outputs of the galileo are shown in the diagram below:


![Galileo outputs](../img/galileo/galileo_outputs.png "Galileo outputs")


The galileo can output two types of signal: *Digital* on/off signals, and *Analog* continuous signals (labelled PWM) - think of it like the difference between a regular light-switch and a dimmer switch.


![Switches, digital and analog](../img/galileo/switches.png "Digital and analog signals")


The board can output *digital* signals on any of its pins (labelled 0-13). It can only output an *analog* signal on pins marked with a "***~***" (pronounced 'tilde'), so that's pins ~3, ~5, ~6, ~9, ~10 and ~11.


## Light-Emitting Diode (LED)
<br>

An LED is a simple example of an analog output: the light can either be off completely or any brightness up to a maximum. LED circuits need a resistor in them in order to limit the current passing through the LED - this stops it from overheating and blowing up! 

It's also important to put the LED in the right way around. You'll notice that one leg of the LED is longer than the other - this end must go on the *positive* side of the circuit, and the other goes on the *negative* end.


![LED output](../img/galileo/Output - LED_bb.png "LED output")


## Servo (includes the robot arm)
<br>

A servo is a lot like a motor, but instead of being designed to turn with as much *power* as possible, it's designed to turn with as much *accuracy* as possible. As a result, it doesn't turn full circle. Instead it turns half a circle, from 0 to 180 degrees.

The robot arms on some of the galileos are just three of these mounted inside a 3d-printed armature. You can decide which inputs control which servos using Connect Anything - try and see if you can pick something up, or do a robot dance!

![Servo output](../img/galileo/Output - Servo_bb.png "Servo output")


## LED ring output
<br>

The LED rings on some of the galileos are controlled by arduino UNOs. This circuit shows you that you can control other microcomputers from your galileo!


The UNO reads the analog signals that you send it, which control the colour and brightness of the LED ring.


![LED ring output](../img/galileo/Output - LED ring_bb.png "LED ring output")


## Audio output
<br>

The speakers on some of the galileos are also controlled by arduino UNOs. They use the [Mozzi library](https://sensorium.github.io/Mozzi/) to generate sounds using the analog signals you send from the Galileo. Hook them up using Connect Anything and see what noises they can make! 


![Audio output](../img/galileo/Output - soundModule_bb.png "Audio output")