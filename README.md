# ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock

This config integrates Voice Assistant with the S3 Box 3's sensor dock.

Features:
  - Voice assistant with on-device and in-HA wakeword
  - Mute VA speech (settings page and red-circle button)
  - Touchscreen
  - IR learning
  - IR blasting
  - Temperature sensor
  - Battery sensor
  - Radar presence detection

## Status Page
![status](https://github.com/AlmostInteractive/ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock/assets/3893631/946a43e4-8dcf-4b96-9e07-71952494b283)

Shows the status of wifi and HA connections, battery charge (if inserted), LED power, and temperature. Shows cute little pictures to depict the VA status.  Nothing interactable.


## IR Learning Page
![irlearn](https://github.com/AlmostInteractive/ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock/assets/3893631/3b4bad68-b882-4eff-b00d-6aa9473ba5f8)

Touch and IR slot button to begin recording to that slot.  Following the on-screen prompts, press the button on your control two times to learn the IR code.  You can record over an existing IR slot.


## IR Blast Page
![irblast](https://github.com/AlmostInteractive/ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock/assets/3893631/a58ba5b2-22e0-438e-8a34-bb098f252465)

Touch an IR slot button to emit the learned IR code.  Note that in my testing the LED emitter was weak.  The device had to be within 1.3m before it would register.


## Voice Assistant Page
![va](https://github.com/AlmostInteractive/ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock/assets/3893631/8a45eaff-bedb-4afe-9b55-1085c55a8ab7)

Shows the complete status of the Voice Assistant, including last STT phrase it heard and TTS reply.  Nothing interactable.


## Settings Page
![settings](https://github.com/AlmostInteractive/ESP32-S3-Box-3-Voice-Assistant-Sensor-Dock/assets/3893631/026f7ec7-4828-437c-8de9-61765ce20ebd)

Allows toggling the VA speaker mute (NB: does not prevent the VA from listening).  Adjust speaker volume and sleep / screen saver delay.


### Resources

https://github.com/BigBobbas/ESP32-S3-Box3-Custom-ESPHome

https://github.com/esphome/firmware/tree/main/wake-word-voice-assistant

https://github.com/AlmostInteractive/ESP32-S3-Box3-IR-Blaster-Learning-Example/
