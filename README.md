# Particle-Boron-Carrier-v1.8
This is a carrier board for 3rd Generation Particle Devices (Boron and Argon).  It is intended to support use in outdoor environments and remote locations.  It includes the following capabilities:
* ESD and Short protection (Fuse, TVS and Varistors)
* Support for Solar charging (Large by-pass cap on DC-In and TMP-32 temp sensor to manage safe charging)
* Programmable Watchdog timer (AB1805)
* Real Time Clock with backup to the main LiPO battery (AB1805)
* On/Off switch using a high-side P-MOSFETS
* User Button for custom usage
* Connectors for IO including compatibility with Spankfun Qwiic and Adafruit Stemma (JST ST/SR)
* Footprint for a LoRA Radio module

![IMG_5598](https://github.com/chipmc/Particle-Boron-Carrier/blob/main/Images/Carrier-v1-8-Top.jpg?raw=true)

![IMG_5599](https://github.com/chipmc/Particle-Boron-Carrier/blob/main/Images/Carrier-v1-8-Bottom.jpg?raw=true)



Key Pin definitions for the FeatherWing Pins
 * Left Side (16 pins)
 Left Side (16 pins)
 * !RESET -
 * 3.3V -
 * !MODE -
 * GND -
 * D19 - A0 -               
 * D18 - A1 -               
 * D17 - A2 -               
 * D16 - A3 -
 * D15 - A4 -               Internal (TMP32) Temp Sensor
 * D14 - A5 / SPI SS -      RFM9x
 * D13 - SCK - SPI Clock -  
 * D12 - MO - SPI MOSI -    RFM9x
 * D11 - MI - SPI MISO -    RFM9x
 * D10 - UART RX -
 * D9 - UART TX -

 Right Size (12 pins)
 * Li+
 * ENABLE
 * VUSB -
 * D8 -                     Wake Connected to Watchdog Timer
 * D7 -                     Blue Led
 * D6 -                     
 * D5 -                     
 * D4 -                     User Switch
 * D3 -
 * D2 -                     RFM9x
 * D1 - SCL - I2C Clock -   FRAM / RTC and I2C Bus
 * D0 - SDA - I2C Data -    FRAM / RTX and I2C Bus


To see minimal code that will exercise the carrier board see this repository:
https://github.com/chipmc/CarrierTest3rdGen


 This board was developed in partnership with the Particle community See this thread for details on this board's development:
 https://community.particle.io/t/boron-xenon-argon-carrier-for-outdoor-applications/48750/213
