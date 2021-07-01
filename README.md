# Adafruit_SSD1306_Microblaze - I2C Fork

**Note:  As of 2021/07/01 - Code has not been verified as functional.  Still a work in progress.**

This is a fork of [jmwilson's repository](https://github.com/jmwilson/Adafruit_SSD1306_MicroBlaze) which itself is a fork of the [adafruit/Adafruit_SSD1306](https://github.com/adafruit/Adafruit_SSD1306) display library.  The former is a port of the latter from the Arduino development environment to the Xilinx Microblaze soft processor (logical processor provided by Xilinx to be flashed on their FPGAs).

This (**my**) repository adds support for I2C SSD1306 OLED displays.  Although the original adafruit code supports both I2C and SPI in Arduino, only SPI is supported in jmwilson's adapted code.  My code will have a constructor each for SPI and I2C instances.  Both instances also require a GPIO interface in your Microblaze configuration for the DC and RST lines.

The default resolution config is 128x64.
