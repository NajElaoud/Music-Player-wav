## Music-Player```.wav```
This project implements a basic audio player using an STM32 microcontroller. It plays .wav files from a USB mass storage device via the I2S interface. External buttons are used to control playback (play/pause, next/previous track) and adjust the volume. The project utilizes:
 + FATFS: For USB file handling
 + I2S: For audio output
 + GPIO Interrupts: To manage button inputs
 + LED Feedback: To indicate button actions

# Features
 + Plays ```.wav``` audio files from USB storage.
 + Button control for Play/Pause, Next/Previous, and Volume Up/Down.
 + LED indicators for each button action.
 + Getting Started

# To use this project:
 + Connect the USB mass storage device with .wav files.
 + Flash the firmware to the STM32 board.
 + Use the buttons to control playback and volume.

# How It Works:
 2. USB Device Connection: Once a USB device is connected and recognized, the system mounts the USB file system.
 2. Audio Playback: The first ```.wav``` file found on the USB is played through the I2S audio interface.
 3. Control Using Buttons:
     - PA0: Toggle between play and pause.
     - PA1: Increase volume.
     - PA2: Decrease volume.
     - PA3: Skip to the next track.
     - PA5: Go back to the previous track.
 4. LED Feedback: LEDs on the board light up for a short duration to indicate button presses and actions taken by the audio player.

# Dependencies:
 + STM32 HAL Libraries: For hardware abstraction and peripherals.
 + FATFS: For file system management on the USB.
 + I2S: For digital audio output to speakers/headphones.

# Hardware Requirements
 + STM32 microcontroller (with USB host and I2S support).
 + USB mass storage device (formatted with FATFS).
 + External buttons and LEDs for control.
 + Audio output (e.g., headphones or speakers).
   
# License
This project is licensed under the terms found in the ```LICENSE``` file. If no license is provided, the software is available as-is.

______________________________________________________________________________________________________________________________________
Feel free to modify and extend the project to suit your needs!
