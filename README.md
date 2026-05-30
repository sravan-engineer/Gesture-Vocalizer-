# Gesture-Vocalizer-
Gesture Vocalizer for Deaf and Mute People using Arduino
Abstract:
Communication is essential in everyday life, but people who are deaf and mute often face difficulties when
interacting with others who do not understand sign language. This project proposes a gesture vocalizer system
using an Arduino microcontroller. A glove equipped with flex sensors detects finger movements and hand gestures.
The sensor signals are processed by the Arduino, which identifies predefined gestures and converts them into
meaningful text or speech messages. The generated message is displayed on an LCD screen and can also be
transmitted through a speaker or Bluetooth module. The system is designed to be simple, low cost, and portable. It
aims to reduce the communication gap between deaf mute individuals and the general public by translating hand
gestures into understandable outputs.
Problem Statement:
Deaf and mute individuals commonly rely on sign language to communicate. However, most people are not familiar
with sign language, which creates a communication barrier in places such as hospitals, schools, and public
environments. Because of this limitation, many basic interactions become difficult. A system capable of translating
gestures into text or speech would significantly improve communication and independence for people with hearing
and speech impairments.
Proposed Solution:
The proposed system uses a wearable glove containing flex sensors that detect finger bending. These sensor
values are read by an Arduino Uno microcontroller through its analog input pins. The program inside the Arduino
compares the sensor readings with predefined gesture patterns. Once a gesture is recognized, the system
generates the corresponding message. The output message is displayed on a 16x2 LCD screen and can also be
converted into voice output using a speaker or sent to a mobile device through a Bluetooth module.
System Block Diagram:
Hand Gesture
↓
Flex Sensors (Finger Movement Detection)
↓
Voltage Divider Circuit
↓
Arduino UNO Microcontroller
↓
Gesture Recognition Program
↓
LCD Display / Speaker / Bluetooth Output
Working Principle:
The glove contains flex sensors attached to the fingers. When the user bends their fingers to perform a gesture, the
resistance of the sensors changes. This change is converted into a voltage signal using a voltage divider circuit. The
Arduino reads these voltage values and compares them with stored gesture patterns. When the values match a
predefined gesture, the Arduino triggers the corresponding message. The message is then displayed on the LCD
screen and can also be produced as audio output through a speaker. This process occurs almost instantly, allowing
real time communication.
Main Components:
Component
Purpose
Arduino Uno
Main controller that processes sensor data
Flex Sensors
16x2 LCD Display
HC 05 Bluetooth Module
Resistors
Battery
Glove
Detect finger bending and gesture movement
Displays the generated message
Wireless communication with phone
Used in voltage divider circuit
Provides power supply
Used to mount sensors on fingers
Component
Cost (INR)
Arduino Uno
Flex Sensors (4)
LCD Display
Bluetooth Module
Resistors & Wires
Glove
Battery
Advantages:
• Helps deaf and mute people communicate easily with others.
• Low cost and easy to implement using Arduino.
• Portable and simple to use.
• Can be extended with mobile applications or AI based gesture recognition
