---
layout: post
title: "Evacuation of South Florida Due to Irma, on a Traffic Cam"
date: 2017-09-13 21:00:00 -05:00
comments: false
---

Hurricane Irma was forcast to hit Miami and work it's way up the whole state. A lot of people decided to leave and there wasn't really any place to go except north. I live in Gainesville, right on one of the two north-south interstates in the state - I75. Our city runs traffic cameras and the make current images available on a [SmartTraffic](http://gac-smartraffic.com/) site. A few months ago I wrote a script to pull all the images once a minute so I have a history of all the "current" images.

I thought it would be fun to stich them together to make a time-lapse video of the interstate. I started it around Sept 1 so you can see normal traffic, the evacuation rush starts around 9/6, and it runs up until the traffic system crashed at 1:45 am on Monday morning which is about 15 minutes after the peak winds were forcast to hit.

Video on Youtube:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/u1P1jwD-Hts" frameborder="0" allowfullscreen></iframe>

Some details about how this was made:

 - The I75 cameras are movable with 4 pre-programmed positions. They take one picture per minute so there's one image about every 4 minutes. You'll also see some times when the camera didn't properly return to it's pre-programmed position.
 - The orientation of the camera isn't saved in the image metadata (who would have thought that would be useful!) but it is displayed in the image. I OCR'ed the orientation from a crop in the image with pyocr and tesseract. It was pretty good but you'll see some stray images from other positions where the OCR messed up. I'm not a tesseract wizard.
 - There are gaps in the images for a number of reasons. Sometimes the camera goes out. Sometimes the images are partial downloads since I'm pulling a jpg off a web server every minute and they're uploading to the same file name every minute. I get about 5% corrupt or partial files.
 - The final image is just the last image uploaded off the camera before it died. It just happened to be in the right orientation so for the last 2 days I was pulling the same image of their web site. Its all a hack.
 
 So far I have download ~40 cameras worth of data since February 2017 every minute for a total of about 750 GB and 16 million images. Not sure what else I'll do with them.
