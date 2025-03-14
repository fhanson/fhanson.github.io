---
title: Building BD-3
category: builds
layout: page
image: /static/BD-3 front side.jpeg
excerpt_separator: <!--more-->
---

Poking around reddit for costume ideas for Awesomecon 2025 I came across a [design for building BD-1 from Jedi: Fallen Order](https://www.thingiverse.com/thing:4078727). I hadn't printed anything this large before but I loved the idea of animating it with lights and sounds. 
After printing a couple of the inital parts I started looking at how others had remixed it to make it unique.
<!--more-->
![]({{ 'static/BD-1_JFO.jpeg' | relative_url }})

My next stop was off to grab some parts from microcenter to get the animation working. I decided on an [adafruit propmaker board ](https://www.adafruit.com/product/5768)since it could do sounds, neopixels and had motion sensitivity. I loaded up Circuit python and began testing turning lights off and on.
With the head printed, I realized I couldn't fit my hands inside to get access to things easily so I needed to make some changes. Splitting the head into a cover and adding magnets gave me the room I needed and while I was at it, I  embedded the amp [power pack from here](https://www.thingiverse.com/thing:4507018).
![]({{ 'static/BD-1 Head Shell.png' | relative_url }})

For printing the body I went with ABS filament to give it some strength and used PLA on areas I thought I could get away with it. 
![]({{ 'static/BD-1 half printed.jpeg' | relative_url }})

Playing with the adafruit board I found I could reuse some of my OLED screens I bought for the lightsaber chassis. They were pretty much plug and play like the Proffie boards. I switched up the [amplifier side plate](https://www.thingiverse.com/thing:6977918) to pressure fit the OLED screen and made a hole in the head cover to run wiring.

Once he was mostly printed I gave him a shot of primer.
![]({{ 'static/BD-1 primer.jpg' | relative_url }})
Unfortunately I had the ankles on backwards, I was able to break them off later without too much damage but I had to reprint a couple of the toe pieces.

Painting BD-3 started out easy enough with some rattlecans I sprayed him an ivory color and decided on forest green accents. The masking I used for the green bled through though so I had quite a bit of touch up work to do. Fortunately I wanted a weathered look anyways so I fixed as much as I could by hand after.
![]({{ 'static/painting BD-3.jpg' | relative_url }})

Once paint dried I began test fitting electronics, adding led's and trying to figure out how best to mount the pixel strips.
![]({{ 'static/BD-3 head.jpeg' | relative_url }})

I ended up with about 36 pixels in the back of his head in two rows and one neopixel for each eye. I also found a nice acrylic lens on amazon that fit his larger eye.
For led animation I couldn't decide on one color so I created a sequence to run through colors and pulses. I tracked down a couple sound clips and added them to run randomly. After a while it started to drive me crazy so I switched that to his more common beeps and added the touch sensitivity for the louder clips.
I made a voltage divider with 10k resistors like on the adafruit site and read out the battery voltage on the screen so I know when to charge him. I also added a kill switch to the main body with the speaker and ran those wires back to the head where the adafruit board sits.

![]({{ 'static/BD-3 back.jpeg' | relative_url }})
![]({{ 'static/BD-3 front.jpeg' | relative_url }})
