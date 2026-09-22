# **Servo Motor Control Using Arduino**

##  **Description**

This project demonstrates how to control the position of a **servo motor using an Arduino**. The Arduino sends control signals to the servo motor, allowing it to rotate to a required angle.

##  **Objective**

* To understand the working of a servo motor.  
* To control servo motor position using Arduino.  
* To learn basic interfacing between Arduino and a servo motor.  
* To develop a simple motor control system.

##  **Components Required**

* Arduino Uno  
* Servo Motor (SG90)  
* Jumper Wires  
* Breadboard  
* USB Cable  
* Computer/Laptop

##  **Working**

The servo motor is connected to the Arduino through its power, ground, and signal pins. The Arduino generates a PWM control signal through a digital pin. Based on this signal, the servo motor rotates to the desired angle, typically between **0° and 180°**.

##  **Connections**

| Servo Wire | Arduino |
| ----- | ----- |
| Red – VCC | 5V |
| Brown/Black – GND | GND |
| Orange/Yellow – Signal | Digital Pin 9 |

##  **Working Process**

**Arduino → Control Signal → Servo Motor → Angular Rotation**

1.Arduino is powered through USB.

2.The servo motor receives power from the Arduino.

3.Arduino sends a control signal to the servo.

4.The servo rotates according to the given angle.

5.Different angles can be programmed using Arduino code

**Program**

\#include \<Servo.h\>

Servo myServo;

void setup() {

  myServo.attach(9);   // Servo signal pin connected to D9

}

void loop() {

  myServo.write(0);

  delay(1000);

  myServo.write(90);

  delay(1000);

  myServo.write(180);

  delay(1000);

}

##  **Conclusion**

The **Servo Motor Control Using Arduino** project provides a simple way to understand motor control and Arduino-based automation. It demonstrates how programmed signals can be used to achieve precise angular movement.

