Wifi jammer
WiFi jamming device.

How to:

Raspberry Pi:

Install Arch Linux. http://archlinuxarm.org/platforms/armv6/raspberry-pi
Install python2, python2-raspberry-gpio, mdk3, i2c-tools.
Put wifijammer.py in /opt/.
Put wifijammer.service in /etc/systemd/system/.
Enable Wifijammer: systemctl enable wifijammer.
Use a aircrack-ng compatible WiFi adapter.

Arduino:
Upload wifijammer.ino to the board.

Wiring:
The Raspberry Pi as master with the Arduino as slave with address 0x04 over I2C.
3 LEDs (red, green & blue) or RGB LED with 23, 24 and 25 pins (use resistors).
Single pole, triple throw switch with it's far throws to 17 & 22 pins and pull the center throw to 3.3v.
