# NFC-Jukebox

This project is my implementation of the Home Assistant NFC Jukebox Tag project.

This implementation uses Apple Music URLS and my Apple TV for the Player / Music service

Included with the ESP Home yaml for the microcontroller RFID scanner are the automations and scripts triggered once the cards have been scanned.

ESP32 S2 Board used: ESP32-S2FN4R2 [Amazon Link](https://www.amazon.com/dp/B0B28LMBKD?ref=ppx_yo2ov_dt_b_product_details&th=1) <- This board requires you to plug the board directly into the home assistant server to flash, it will not flash over the air or through a computer connected to the interface.\
RFID scanner board: PN532 NFC NXP RFID Module V3 [Amazon Link](https://www.amazon.com/dp/B01I1J17LC?psc=1&ref=ppx_yo2ov_dt_b_product_details)\
3D Printed enclosure: Custom [Onshape Link](https://cad.onshape.com/documents/ec66925a9cd6c534a0f8a11c/w/35f4ecaeaa0d44f1f4ac2f7e/e/4fb00e4a5a71fa35d0e48957?renderMode=0&uiState=666202da0030f31e6bcef69d)
 - Print 1x Base and 1x Lid
 - Plastic Standoffs used for board mounting\
   
Also used in this project is a generic piezo buzzer

Pins used for I2C connection between ESP and RFID:
 - SDA: GPIO18
 - SCL: GPIO21
 - frequency 400kHz

Pins for buzzer:
 - GPIO16
