# gf-tsutenkaku
## arduino, arduino.js, led, weather, browser
This document is made by [gitfab](http://gitfab.org)
---
#Movie
<video src="http://www.mecha-mozilla.org/projects/tsutenkaku//tsutenkaku.theora.ogv" poster="http://www.mecha-mozilla.org/projects/tsutenkaku//thumbnail.jpg" controls="" width="300"></video>
---
#Abstract
Although we can see information of web in web browser, if it is retrieved same information into real world, we can get different experiment. Tsutenkaku is application that we can perceive the area and weather from browsing web page(now Osaka only.. ) by LED which is builtin the photo of Tsutenkaku Tower. It is very simple, but we can see the web information, so we may be able to say it is web browser as well.
---
#Setup for Firefox Addon
Please click [tsutenkaku.xpi](https://raw.github.com/dadaa/gf-tsutenkaku/master/gitfab/resources/tsutenkaku.xpi) on Firefox.
---
#Setup for Arduino
Uploads [CommandServer.ino](https://raw.github.com/dadaa/arduino.js/master/core/sketch/CommandServer/CommandServer.ino) to Arduino.
---
#Setup for Hardware

components

* Arduino
* Multi-Color LED
* Resistor 100Ω x 2
* Resistor 150Ω x 1
* Breadborad
* Jumper lines

![IMG_3929.jpg](https://raw.github.com/dadaa/gf-tsutenkaku/master/gitfab/resources/IMG_3929.jpg)


After all, connects Arduino and PC.
---
#Usage
Please browse as usual in Firefox that is installed the addon. If the url contains a word "osaka", starts to light the LED by weather.

* green &gt; sunny
* red &gt; cloudy
* blue &gt; rainy
---
# Implementation
under construction..
---
#License
<a rel="license" href="http://creativecommons.org/licenses/by/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="width: 100px; border-width:0" src="http://i.creativecommons.org/l/by/2.1/jp/88x31.png"></a>

source code : [MPL2.0](http://www.mozilla.org/MPL/2.0/)

---
#References
* [homepage](http://www.mecha-mozilla.org/projects/tsutenkaku/)
* [tsutenkaku Addon source code](https://github.com/dadaa/tsutenkaku)
---
