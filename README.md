# Home Assistant Assist Hardware

Configuration and stuff for hardware setups for Home Assistant voice assistants.

# M5 Stack Atom Echo

Configuration for the [Atom Echo](https://docs.m5stack.com/en/atom/atomecho) based on ESPHomes original config. A bit simplified and only using push-to-talk right now.

# M5 Stack Atom S3 Lite

Currently WIP!

Should be more powerful, with better sound quality. Build with these components:

- [AtomS3 lite](https://docs.m5stack.com/en/core/AtomS3%20Lite)
- [Atom Speaker Unit](https://docs.m5stack.com/en/atom/atom_spk)
- [Microphone Unit](https://docs.m5stack.com/en/unit/pdm)
- A push external button
- RGB LEDs

TODO-List:

- [X] Basic Setup with WiFi and HA integration
- [X] IR LED
- [X] RGB-LED
- [X] External I2S speaker
- [X] MediaPlayer
- [?] External I2S microphone (WIP)
- [ ] Assist pipeline
- [ ] External Push Button
- [ ] Assist Settings Gain, Noise, Volume
- [ ] LED depending on Assist
- [ ] Additional LED Strip for effects?

# ESP32 NodeMCU

Currently heavy WIP!

Playing around with a unused NodeMCU. Maybe I will used it instead of the AtomS3, but not sure yet
