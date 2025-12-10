---
title: ICM Final
draft: false
tags:
  - ICM
  - p5js
  - FinalProject
  - Homework
---
 
SSTV editor
https://editor.p5js.org/Oremoose/full/pJU8rJXZG

I want to use the audio features of p5js to allow someone to manipulate images via the SSTV audio files. 

The encoding format I will use is the robot36 which renders 320x240 RGB Images.

# Prework
Before I dove into making this project I wanted to have a proof of concept.
I did this by taking four Monet paintings of haybales.
I used [this encoder site](https://www.vr2woa.com/sstv/) to encode the images into the sound files.
then in Audition I took them and sliced them into one file.
![[Screenshot 2025-12-03 131842.png]]

I then fed the sound file into [this decoder site](https://sstv-decoder.mathieurenaud.fr/)

And the Image came out as such
![[decoded-image.png]]

# Time to Get to work
Things need:
1.  Peoples Faces
2. Write the code

I failed immediately. The code I wrote was not accepting the audio library commands. 
I shot Shawn an email and I found out the version of p5.js I was working with did not have a sound library. Additionally I made a post on the Community discord to see if anyone was available for me to take their picture. Alas no one volunteered.

I persisted. Shawn pointed me to the right version of the p5 and I turned to my siblings for selfies.

## Smacking my keyboard
 The way that the sketch works is that.
 1. You click begin recording and then a random file will begin
 2. then you choose 3 splices to play when the timer hit 0
 3. then you click stop recording 
 4. then you click save
 5. then you decode your image.

For the choosing of the splices I used a simple rollover code we learned early in class.
For the Buttons I use the HTML Dom code
for the audio files I used the sound library to jump to the proper locations in the files that would coordinate with the roll over splices.

in the end I was able to take these selfies

![[Screenshot 2025-12-09 223838.png]]

and make this
![[decoded-image (1).png]]
and 
![[decoded-image (2).png]]