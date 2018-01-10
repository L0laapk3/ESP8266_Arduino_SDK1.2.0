# ESP8266_Arduino_SDK1.2.0
How to compile esp8266 programs on arduino IDE with old SDK version 1.2.0 before nerf.

leaving this here as a reference for myself

1. In arduino directory
```
cd hardware
mkdir esp8266com
cd esp8266com
git clone https://github.com/esp8266/Arduino.git esp8266
cd esp8266
git checkout cd69be7f8f56231605e3f9680ac68a095bd77185
```
2. add board to boards.txt, copy text from newest release
3. copy "variants" and "package" folders from newest release into yours

4. copy "tools/get.py" from newest release and execute
5. copy "tools/esptool/esptool.exe" to "tools/esptool.exe"

6. if compile error about "eagle.flash.1m0.ld" set flash size to 64k spiffs
