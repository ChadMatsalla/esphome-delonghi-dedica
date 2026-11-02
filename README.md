
The Problem

The Dedica needs time to warm up and my method requires a second button press. Both of these things take time, so I found that automating it was interesting. The first button press from Home Assistant wakes the machine, the second makes the first part of my coffee, and the third completes the process. Then later when it's time for the next cup I repeat.

The Approach

ESP32 with esphome, Homeassistant.

The Hardware

In previous versions I used the relay board because my partner wanted both the 'single drop' and 'double drop' buttons to be operated. That was very clunky. I since designed a circuit board with 2 transistors to close the circuit to press the buttons. Much smaller and easier.

For people who want to automate one of the buttons and are uncomfortable with wiring or soldering, I've been happy to use M5 Stack products. I'd recommend the [M5 Atom-Lite](https://docs.m5stack.com/en/core/Atom-Lite) or something even smaller like the [C125 Nano C6](https://docs.m5stack.com/en/core/NanoC6)and the [U023 M5 unit relay](https://docs.m5stack.com/en/unit/Unit_Relay). If you need to control both buttons you can use the [U131 Unit 2Relay](https://docs.m5stack.com/en/unit/Unit_2Relay). *DO NOT USE ARDUINO, use esphome*





Delonghi Dedica EC680M
![Delonghi Dedica](/images/delonghi-dedica.jpg)

ESP32, ESP8266, Arduino, Raspberry Pi, or any device with GPIOs
- I used a Lolin D32 like this:
![Lolin D32](/images/lolin-d32.jpg)

Relay module
- I used a generic relay module like this:
![Relay Module](/images/relay-module.jpg)

Waterproof butt connectors
![Waterbproof Butt Connectors](/images/waterproof-butt-connectors.jpg)
