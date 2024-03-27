# Home Assistant Assist Hardware

Configuration and stuff for hardware setups for Home Assistant voice assistants.

## M5 Stack Atom Echo

Configuration for the [Atom Echo](https://docs.m5stack.com/en/atom/atomecho) based on ESPHomes original config. A bit simplified and only using push-to-talk right now. No additional hardware necessary!

## ESP32 DevKit

A bigger variation with different components:

- ESP32 DevKit V4
- INMP441 I2S Microphone
- MAX98357 I2S Amplifier with 3W Speaker
- LED Strip with 32 addressable LEDs
- I2C OLED
- Push-Button for Push-to-Talk

Pinning:

- GPIO2 - LED (Listening)
- GPIO4 - INMP441 SO
- GPIO13 - Push Button
- GPIO15 - LED (Mute)
- GPIO18 - LED Strip CLK
- GPIO21 - OLED SDA
- GPIO22 - OLED SCL
- GPIO23 - LED Strip Data
- GPIO25 - MAX98357 DIN
- GPIO26 - INMP441 WS
- GPIO27 - INMP441 SCK
- GPIO32 - MAX98357 BCLK
- GPIO33 - MAX98357 LRC

Additional connections:

- INMP441 L/R: GND
- MAX98357 GAIN: Not connected
- MAX98357 SD: Bridge to VDD (Channel Left selected)

## ESP32-S3

I use a chinese clone of Espressifs ESP32-S3-DevKitC with slightly different pinning. The on-board RGB-LED is at IO48 instead of IO38 for example.

Pinning:

- GPIO1 - OLED SDA
- GPIO2 - OLED SCL
- GPIO4 - LED Strip CLK
- GPIO5 - LED Strip CLK
- GPIO6 - LED 1 (Mute)
- GPIO7 - LED 2 (Listening)
- GPIO9 - MAX98357 BCK
- GPIO10 - MAX98357 DIN
- GPIO13 - Push Button
- GPIO19 - INMP441 SO
- GPIO20 - INMP441 WS
- GPIO21 - INMP441 SCK
- GPIO46 - MAX98357 DIN
- GPIO48 - On-Board RGB-LED

- INMP441 L/R: GND
- MAX98357 GAIN: Not connected
- MAX98357 SD: VDD (Channel Left selected)

DONE:

- Basic Setup with WiFi and PSRAM
- OnBoard RGB-LED
- Push-Button
- LED Strip
- LED Listening
- LED Mute
- OLED
- Microphone
- Speaker (Not working with ESP-IDF?)

TODO:

- I2S: 22pF against GND
- Move to ESP-IDF
- microWakeWord
- Choose between WakeWord and push2talk with a switch
- Mute-Button
