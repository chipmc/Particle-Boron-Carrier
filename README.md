# Particle-Boron-Carrier-v1.6
This is a carrier board for 3rd Generation Particle Devices (Boron and Argon).  It is intended to support use in outdoor environments and remote locations.  It includes the following capabiltities:
* ESD and Short protection (Fuse, TVS and Varistors)
* Support for Solar charging (Large by-pass cap on DC-In and TMP-32 temp sensor to manage safe charging)
* Programmable Watchdog timer (AB1805)
* Real Time Clock with backup to the main LiPO battery (AB1805)
* On/Off switch using a high-side switch for transit and storage (TI TPS22810)
* User Button for custom usage
* Connectors for IO including compantibility with Spankfun Qwiic and Adafruit Stemma (JST ST/SR)
 
![IMG_5598](https://user-images.githubusercontent.com/6188397/113896743-38480800-9798-11eb-91e1-d70a0c5279e2.jpeg)

![IMG_5599](https://user-images.githubusercontent.com/6188397/113896760-3bdb8f00-9798-11eb-9fd7-45b0ed94a1b0.jpeg)

Key Pin definitions for the FeatherWing Pins
 * Left Side (16 pins)
 * !RESET
 * 3.3V Out (up to 1000mA including Boron's demand)
 * !MODE Button (mirrors button on Particle device)
 * GND
 * D19 - A0
 * D18 - A1
 * D17 - A2
 * D16 - A3
 * D15 - A4 - TMP32 Temp Sensor
 * D14 - A5 / SPI SS 
 * D13 - SCK - SPI Clock
 * D12 - MO - SPI MOSI
 * D11 - MI - SPI MISO
 * D10 - UART RX
 * D9 - UART TX

 Right Size (12 pins)
 * Li+
 * ENABLE
 * VUSB - Connected to the same USB power as the microUSB port on the Boron
 * D8 -   Wake Connected to Watchdog Timer
 * D7 -   Blue Led on Particle device
 * D6 -   DEEP-SLEEP Enable Pin - Brings Enable Pin low - Only RTC Alarm interrupt will wake
 * D5 -   Done Pin Connected to the Watchdog Timer
 * D4 -   User Switch
 * D3 - 
 * D2 - 
 * D1 - SCL - I2C Clock -   FRAM / RTC and I2C Bus
 * D0 - SDA - I2C Data -    FRAM / RTC and I2C Bus

To see minimal code that will exercise the carrier board see this repository:
https://github.com/chipmc/CarrierTest3rdGen

 
 This board was developed in partnership with the Particle community See this thread for details on this board's development:
 https://community.particle.io/t/boron-xenon-argon-carrier-for-outdoor-applications/48750/213
