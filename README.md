# Basic example of using arduino-mqtt in a class

If you want to progress beyond a single code file for your MQTT project, you'll likely need to implement it as part of a larger codebase. This project will help you understand how to use the more advanced features of the great [arduino-mqtt by 256dpi](https://github.com/256dpi/arduino-mqtt).

In the Connectivity-class, you'll find features to connect to wifi, connect to the test.mosquitto.org broker, subscribe for a topic, print out messages to the topic, send status messages and stay connected. To use the example, you'll have to edit the wifi settings in Connectivity.h. You can also change the MQTT details here if you want to a different mqtt broker/server.

## Using with Platformio

This repository is a full project for Platformio that can easily be cloned/downloaded and setup locally. It's using an Adafruit Feather Esp32-S3 with no psram as a default, so you'll need to edit the platformio.ini if you use a different ESP32 based development board. If you use something other than an ESP32, you'll likely need to change the wifi connection a bit.

## Using the example with Arduino IDE

If you are using the Arduino IDE, you'll only use what's in the /src/ folder. Copy the folder and it's content and rename the folder "basicmqtt". Then change the name of "main.cpp" to "basicmqtt.ino". You will also need to install the arduino-mqtt library by 256dpi using the Library manager in the Arduino IDE.
