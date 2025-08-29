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


<video src="https://dashby1.github.io/Portfolio/photos/GasPacsPhotos/0422212234.mp4" controls width="200px" height="250px" id="CSGSV1"></video>
I also designed and built a controller interface board which takes in serial input from a PC and triggers an antenna rotor to move. This allowed us to controll the rotor with a few dollars worth of components rather than spending a few hundred dollars for an ots rotor controller. This being my first electronics project ever, i am still very proud of it. The video to the left shows and initial protoype and testing, only one direction is hooked up, Once this was shown to work I hooked up all 4 direction controlls (+/- azimuth and +/- elevation). The program uploaded to the arduino is a lighly modified version of the [K3NG project](https://blog.radioartisan.com/arduino_rotator_controller/) which was very convienient as it has live satellite tracking built in which simplified the setup immensly.


Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<img src="https://dashby1.github.io/Portfolio/photos/GasPacsPhotos/0525210901.jpg" width="200" height="300" id="CSGS2">

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].



[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
