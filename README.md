# LightningNetworkPCB
This is a lightning network esp32S2 experimentation PCB (POS/ATM)
Licence is GPL3 I never read :) But philosophy is: do what you want with it. 
If you want to encourage me, here is my BTC wallet address: bc1qdy8alfz6t623trqzk2m0mzrz8w87wwgjc9azgc
My LN Wallet: lnbc1p38nqhcpp5dr46a44fh3jh4uhenvvuxhza30jzzg2auevfjff3hw0uxne34k8qdqu2askcmr9wssx7e3q2dshgmmndp5scqzpgxqyz5vqsp5hzff9unn0vs4f9qsam9a67ffl5hydvs7n4yxd2n6f3aa29qd9jks9qyyssq4y6nllz8ku0qk05glep3g6frwyypptjahnv4t9neszszl07pl944seglzcfk7q9hreuq62wl3f8jjn4ugytncnhhm3zngr34ektzegspkv3cxk

This board is using
An ESP32-S2 wroom chip from espressif
A 2.8 inch touch screen (ILI9341 SPI)
A 3x4 keypad

You have a connector for the CH-926 Coin selector. Have a look at the PCB writing (the wiring is explained)
The CH-926 coin pin is 5V. I built a level shifter to be able to talk to the ESP32 pin in 3.3v

You also have a bunch of extra GPIO / SPI and I2C connector on the top back of the PCB. It allows you to connect a TTL thermal printer, should you want to create a LN-POS
You also have extra ESP32-S TRX1 TRX0 pins to talk to another devive thru UART. I have added these to be able to talk to a CAM-ESP32, should you want to read QR code from another ESP32 device
You hace I2C SDA/SCL pins to connect, for instance, a NFC reader/writer to process payments.


Have fun

Dr Philippe CADIC
pcadic(at)gmail.com

