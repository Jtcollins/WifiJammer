Wifi jammer
WiFi jamming device.

How to:

Raspberry Pi:

Install Arch Linux as described here http://archlinuxarm.org/platforms/armv6/raspberry-pi
Install python2, python2-raspberry-gpio, mdk3, i2c-tools packages.
Place wifijammer.py in /opt/.
Place wifijammer.service in /etc/systemd/system/.
Enable the Wifijammer service: systemctl enable wifijammer.
Plug any aircrack-ng compatible WiFi adapter (I used TL-WN722N).

Arduino:
Upload wifijammer.ino to the board.

Wiring:
The Raspberry Pi as master with the Arduino as slave with address 0x04 over I2C, there is tons of tutorials on how to do this.
3 LEDs (red, green & blue) or RGB LED with 23, 24 and 25 pins (limit their current with resistors).
Single pole, triple throw switch with it's far throws to 17 & 22 pins and pull the center throw to 3.3v.
LCD display with the Arduino like this: http://arduino.cc/en/Tutorial/LiquidCrystal