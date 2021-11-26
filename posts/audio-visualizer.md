# Audio Visualizer
{: .no_toc }
[GitHub repo](https://github.com/robbieculkin/RGB-LED-Audio-Visualizer)

## Demo
<iframe width="560" height="315" src="https://www.youtube.com/embed/it2vcdtha2U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

1. TOC
{:toc}

## Materials
* Arduino Mega
* Solderless Breadboard w/ power rails
* Sparkfun Spectrum Shield (2 MSGEQ7s on a shield)
* Adafruit NeoPixel White 60 LED strip - 3 meters
* Toggle Switch x2
* 5V 10A Power Supply (you can get away with a much lower amperage supply, but you might get some color inaccuracies)
* 9V 650mA Power Supply
* Female DC barrel adapter
* 4700uF 10v Electrolytic Capacitor
* 220 ohm resistor x2
* Stranded-core wire - 6 meters
* 3.5mm audio cable (aux cord)

This could be done with cheaper components, however many of these parts came leftover from other projects.

## Wiring

The [original schematic](https://github.com/robbieculkin/RGB-LED-Audio-Visualizer/blob/master/2-strip%20RGB%20LED%20schematic.fzz) is now out-of-date. Higher amperages can fry smaller solderless breadboards due to arcing between rails. I routed all power to LEDs off the breadboard, opting for direct 5V connections between power sources and LED strips.

I used 2 toggle switches, one for 9V power to the Arduino and one for 5V power to the strip. While not in the schematic, I used two female DC barrel adapters for the 5V and 9V supplies. I used stranded-core wire for flexibility, but found them a nuisance when plugging into the breadboard. My solution for this: add some solder to the end of the wire. This gave me the convenience of a solid-core with the flexibility of a stranded-core. 

I used 2 male-male 3.5mm cables that plug directly into the Sparkfun Spectrum Shield.


## Code

[GitHub repo](https://github.com/robbieculkin/RGB-LED-Audio-Visualizer)

The bulk of my time was spent tweaking animations. I started with a stuttered, basic animation that I slowly fine-tuned over the course of my freshman winter term at SCU. 

