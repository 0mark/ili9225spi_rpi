# ili9225spi_rpi
ILI9225 SPI TFT Library for Raspberry


This is library for RaspberryPi.   
This library can show a chart to ILI9225 SPI TFT.   

----

Wirering   

|TFT||Rpi/Opi|
|:-:|:-:|:-:|
|MISO|--|N/C|
|LED|--|3.3V|
|SCK|--|Pin#23|
|MOSI|--|Pin#19|
|D/C|--|Pin#3|
|RES|--|Pin#5|
|CS|--|Pin#24|
|GND|--|GND|
|5V|--|5V|

----

build   

wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.42.tar.gz   
tar zxvf bcm2835-1.42.tar.gz   
cd bcm2835-1.42   
./configure   
make   
sudo make check   
sudo make install   
cd $HOME   
git clone https://github.com/nopnop2002/ili9225spi_rpi   
cd ili9225spi_rpi   
cc -o demo demo.c fontx.c ili9225.c -lbcm2835 -lm   

---

![ili9225-3](https://cloud.githubusercontent.com/assets/6020549/25643234/827c5e60-2fd9-11e7-8f3d-969950c99615.JPG)
