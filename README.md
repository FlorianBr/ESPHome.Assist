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

TODOs:

- Choose between WakeWord and push2talk with a switch
- Mute-Button
- Use ESP-IDF instead of Arduino
- Port to ESP-C3
