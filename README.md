RaspiRoverDuino
============
Integration Dagu 5 Rover 4x4 with Arduino and Raspberry PI via Node.js

<img src="https://www.codeship.io/projects/c98e3610-59a2-0131-2375-221ce794439b/status"/>

Hardware
--------------

- <a href="http://www.pololu.com/product/1551">Dagu Rover 5 Tracked Chassis with Encoders</a> 
- <a href="http://robosavvy.com/store/product_info.php/products_id/1573">Dagu - 4 Channel DC Motor Controller with Encoder Support</a>
- <a href="http://www.pololu.com/product/1547">Expansion Plate</a>
- <a href="http://www.element14.com/community/community/raspberry-pi">RaspBerry PI Model B</a>
- <a href="https://www.modmypi.com/w311u-high-gain-long-range-wifi-dongle">WiFi Dongle - Tenda W311U+ High Gain 3.5dB</a> 
- <a href="http://www.ebay.it/itm/Neu-Camera-Module-Board-5MP-Webcam-Video-1080p-720p-fur-Raspberry-Pi-/380746393772?pt=DE_Computer_Sonstige&hash=item58a640e8ac">RaspiCam</a>
- <a href="http://www.4tronix.co.uk/arduino/Pan-Tilt-Micro.php">Pan Tilt Cam</a>
- <a href="http://store.arduino.cc/index.php?main_page=product_info&cPath=11_12&products_id=195">Arduino UNO R3</a>
- 9 Volt Battery for Dagu - 4 Channel DC Motor Controller
- <a href="http://callpod.com/products/fueltank">CallPod - Fueltank UNO for Raspberry PI</a>
- <a href="http://www.ebay.it/itm/130995862894?ssPageName=STRK:MEWNX:IT&_trksid=p3984.m1497.l2649">Snap Clip 9V Battery</a>
- <a href="http://www.ebay.it/itm/Arduino-Breadboard-Jumper-Cable-Wires-65-Cable-Pack-/140922066946">Jumper Cable</a>
- MPU6050
- HC-SR04

App Configuration
--------------
- Node.js
- Express.io
- configuration file on /app/conf/index.js

SW Configuration
--------------
- <a href="https://www.modmypi.com/blog/how-to-set-up-the-ralink-rt5370-wifi-dongle-on-raspian">WIFI configuration</a>
- <a href="http://daringfireball.net/projects/markdown/basics">Node.js</a>
- <a href="http://www.raspberrypi.org/camera">Raspi Camera</a>
- <a href="http://www.miguelmota.com/blog/raspberry-pi-camera-board-video-streaming/">RaspiCam Stream</a>
- <a href="https://github.com/jacksonliam/mjpg-streamer">Plugin Raspi Camera very fast stream!!</a>
- <a href="http://blog.bitify.co.uk/2013/11/interfacing-raspberry-pi-and-mpu-6050.html">MPU5060</a>

TO DO

HW Configuration
--------------

Arduino Library
<a href="https://code.google.com/p/arduino-new-ping/">ping HC-SR04</a>

Arduino Pin

LEFT_FRONT Motor
Pin 3 - CHANNEL 1 PWD PIN - analogwrite modulation
Pin 2 - CHANNEL 1 DIR PIN

RIGHT_FRONT Motor
Pin 5 - CHANNEL 3 PWD PIN - analogwrite modulation
Pin 4 - CHANNEL 3 DIR PIN

LEFT_REAR Motor
Pin 6 - CHANNEL 2 PWD PIN - analogwrite modulation
Pin 7 - CHANNEL 2 DIR PIN

RIGHT_REAR Motor
Pin 9 - CHANNEL 4 PWD PIN - analogwrite modulation
Pin 8 - CHANNEL 4 DIR PIN

Cam Tilt pannel
Pin 13 - Left-Right
Pin 12 - Upper-Down



Expansion Plate
- Cut expansion plate with two holes under the engine controller to pass the 4 motor connectors

TO DO

Images
--------------

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/interface_2.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2273.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2274.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2275.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2276.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2277.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2278.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2279.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2280.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2281.jpg"/>

<img src="https://raw.github.com/marcoberri/mbraspiroverduino/master/image/IMAG2282.jpg"/>

Video
--------------

<a href="https://www.youtube.com/watch?v=3kZttU3sqc0">First Test</a>

NOTE
--------------
- the app on nodejs not support socket.io in clutering mode (see server.js in root folder)
- for streaming see this article <a href="https://github.com/jacksonliam/mjpg-streamer">Plugin Raspi Camera very fast stream!!</a>

TO DO
--------------
- configure gyro
- test on mobile phone
- change raspberry to hotspot wifi.
- add ping sensor