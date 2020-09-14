# miro_arduino_ide_dfu
Arduino IDE patches for MIRO wireless Arduino firmware upload support

# Content
"patсh/win" and "patch/linux" - Put files from this folder to your arduino ide root folder.

# Manual
1. Download ARDUINO IDE: https://www.arduino.cc/en/Main/Software

2. Unpack/install ARDUINO IDE

3. Put files from "patсh/win" and "patch/linux" to your ARDUINO IDE root folder

4. Run ARDUINO IDE and install ESP8266 tools with this manual: https://arduino-esp8266.readthedocs.io/en/2.5.2/installing.html. You need to install ESP8266 Arduino Core v2.6.0(!!! only this version is guaranteed to work completely).

4. From Sketch->Include Library->ManageLibraries... find and install ArduinoJson v5.x.x by Benoit Blanchon

5. Restart ARDUINO IDE

In you have error in Arduino IDE in Linux on sketch upload, you need to give rigths for arduino_mcuota executable file:

`$> cd <arduino_ide_root_folder>/hardware/tools/avr/bin`

`$> chmod +x arduino_mcuota`
