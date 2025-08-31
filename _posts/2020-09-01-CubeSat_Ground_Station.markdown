---
layout: post
title:  "CubeSat Ground Station"
date:   2020-09-01 01:23:46 -0700
# image: /photos/GasPacsPhotos/0525210901.jpg
categories: projects
---
The GAS team, USU's amatuer satellite design team was the first design team I as a part of when I went to USU. I joined almost immediatley during my freshman year in the fall of 2020 and stayed until March of 2022.

During my time on the team, I quickly got promoted to the communications team lead just 3 months after joining. My main duty was building a functional ground station to communicate with the GASPACS cubesat which launched in December 2021.


<img src="https://dashby1.github.io/Portfolio/photos/GasPacsPhotos/0525210901.jpg" width="200" height="300" id="CSGS1">

My first responisbilities on the team was to make a link budget for the radio transmissions. This was challenging as I had no experience or knowledge about satellite communication, RF theory, or radios for that matter. Luckilly for me, making the link budget was relativley simple as I came to learn it was just the sum of all the decibel gains and losses of the system, which the main loss be easily calculated easily from the planned altitude of mission and most of the gains can be found on any amplifier and antenna datasheet which we already had.


<video src="https://dashby1.github.io/Portfolio/photos/GasPacsPhotos/RotorVideo.mp4"  id="CSGSV1" width="540" height="675" controls></video>
I also designed and built a controller interface board which takes in serial input from a PC and triggers an antenna rotor to move. This allowed us to controll the rotor with a few dollars worth of components rather than spending a few hundred dollars for an ots rotor controller. This being my first electronics project ever, i am still very proud of it. The video to the left shows and initial protoype and testing, only one direction is hooked up, Once this was shown to work I hooked up all 4 direction controlls (+/- azimuth and +/- elevation). The program uploaded to the arduino is a lighly modified version of the [K3NG project](https://blog.radioartisan.com/arduino_rotator_controller/) which was very convienient as it has live satellite tracking built in which simplified the setup immensly.


With a RTL-SDR stick, a cheap low noise amplifier, and a hand held dual HF/UHF yagi antenna, I as able to gather downlinks from noaa and goes satellites and even a few transmissions from the ISS. Putting this recieving setup on a cart with the antenna rotor, a much larger antenna, and a portable power supply we had a mobile ground station that we could store inside but also make quick changes to our setup. 

Near the middle of the summer of 2021 we got a room with roof access and made a permanent setup and ground station/comms room for satellite transmissions. With this we updated our LNA to one with much higher gain and with an outdoor rating, a HF/UHF dueplexer, and a much larger coax cable. In addition we also setup our groundstation with the satnogs groundstation network which can be seen [here](https://network.satnogs.org/stations/2550/)

The main purpose of this ground station was to recieve transmissions from the GASPACS cubesat and I also think it was to meet a grant requirement? The GASPACS cubesat was setup to transmit on 437.365 MHz suing GFSK modulation. It also transmitted an audio beacon of a clip of the USU Scotsman every few minutes. In December of 2021, the GASPACS cubesat was launched to the ISS and was deployed from the ISS the following January. Right after the deployent we were able to get confirmation that the satellite was operating by the audio beacon. Soon after we were able to transmit commands and get downlinks of telemetry data and images.

<img src="https://dashby1.github.io/Portfolio/photos/GasPacsPhotos/0525210901.jpg" width="200" height="300" id="CSGS2">
