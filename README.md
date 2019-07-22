# esp8266-AC-control
This is just a web interface for the IRremoteESP8266 library made by @crankyoldgit witch will allow you to controll most of AC units from the market.

## Instructions:

 - Connect IR led to one GPIO pin (recommended pin is D2)

 - Edit esp8266-AC-control.ino header marked as "User space". You will need to import the library dedicated for your AC model. Every library has its own commands for AC mode and fan speed that will need to be replace according to commands available in .h file of the library.

 - Flash the firmware in ESP board using 1M or 2M of SPIFFS storage.

 - Connect the board to yout wifi network (look for "AC Remote Control" SSID and follow WiFi Manager wizard)

 - Upload web application files in SPIFFS storage using build in web form located at /file-upload path.

## DEBUG:

Use mobile phone cammera to see if the led send any IR signals. This will show if the circuit was properlly made and the selected GPIO pin is the correct one.


## Credits:

Interface: https://github.com/ael-code/daikin-control  
IR library: https://github.com/crankyoldgit/IRremoteESP8266
