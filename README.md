# Cybersecurity : CSN150
Project: ESP32 XXXXXXXX (FOAD)

## Purpose
Set up ESP32 and Arduino enviornment. Execute sketch " Wifiscanner". 

## Equipment
* [ESP32Cam](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)

* [USB Micro Data Cable](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_sspa?keywords=micro+usb+data+cable&qid=1678902214&sprefix=Micro+USB+data+%2Caps%2C89&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFaU0NaUVZHU1RFUlAmZW5jcnlwdGVkSWQ9QTA3NTA4MDVFVERCS01HVlgxM1YmZW5jcnlwdGVkQWRJZD1BMDE4NTE1NTIwWUdONkdWSzU1M1Amd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

## Links to documentation and tools

##### Video 1: 

##### Other Links: 
 https://www.arduino.cc/en/software/
 
##### AI GPTs used

## Steps I followed
1. Write the steps you followed here.  This way you can keep track of where you might have messed up if the project does not work. 
1. Install Arduino IDE 2.3.10
2. Connect camera and install all necessary drivers.
3. Added the ESP32 board to Arduino IDE by going to file>preferences>additional boards manager URLs and pasted "https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json" in the box and clicked OK.
4. Moved to the board icon on the left side and clicked it. The board manager opened and i typed "esp32" in the search bar. Selected the entry "esp32 by Espressif Systems" and  clicked on install and waited till it finished installing.
5. Clicked on the dropdown menu at the top and select the “Select Other Board and Port” entry. In the search bar i typed esp32 and clicked the search icon.
6. Clicked on the AI thinker esp32 CAM and clicked the COM5
7. To make sure everything is sset is perfectly, i tested using the classic blink example.
8. Moved to file>example>basics>blinks
9. In the code, i replaced the 'LedPin' to 4.
10. After ruuning it, the led started blinking.
11. 
## Problems and Solutions
Note your problems or errors here.  Google any error you may come across, and not what you tried (even if it does not work), and what was the final answer. Document your errors and solutions that worked for you.  

**Problem:** E (485) camera: Camera probe failed with error 0x105(ESP_ERR_NOT_FOUND)
Camera init failed with error 0x105
**Solution:**

### Example Problem
**Problem:** Arduino code will not load on ESP32 Cam.
**Solution:** Camera drivers were incorrect I needed to install the driver: [https://www.wch-ic.com/downloads/CH341SER_ZIP.html](https://github.com/martin-ger/esp32_nat_router).  I used file, "CH341SER.ZIP" and it worked.

## Final Report
