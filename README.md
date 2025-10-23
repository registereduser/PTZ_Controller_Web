This project is to enable controlling a RS485 connected PTZ camera from a web site.
It will probably evolve over time, for now it can control using Pelco D and ForwardVision for Old Bosch Mic400 cameras.

It was initialy deployed on a ESP8266 but did not perform well, upgrading to ESP32 Wroom performed better.

To Release a new version:
  Compile the new build from Arduino IDE with the increased version number.
  Export the bin file
  Upload the .bin file as firmware.bin over writing the previous version.
  Update the firmware.version file with the new version number in it e.g. 1.1
  Open ptz_zoom2.html in a browser, wait for mqtt connection and observe the PTZ connecting and reporting the new version.
