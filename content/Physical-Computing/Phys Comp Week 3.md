---
title: Physical Computing  Week 3
draft: false
tags:
  - ClassNotes
  - Physical-Computing
---
## Class Notes:

Zoom class.

Get more details for the labs when possible.
If we are covering something that we already know. experiment and push our knowledge.

Read Kate's Blog - fish wire

Fritzing http://fritzing.org/ - Used to make circuits digitally.


The analogue pins out put do not simply put out 

Code reference:
https://docs.arduino.cc/language-reference/#functions

Tom's Tone Repo:
https://tigoe.github.io/SoundExamples/

servo motor yellow line listens for the signal. 

if the uploading is failing double tap the reset button on the board that will stop all inputs and out puts on the board and waits for upload. 
## Homework:

Do the basic of the labs then make a controller of analog output from our own design 

I want to make a breathing RGB LED - this did not work because the LED that I have shared cathode and so I cannot change which pin gets power.

### Labs

#### Speaker:
I had a few hiccoughs to tackle:
1. I had did not realize that the speaker needed wires attached to it. 
   Not having alligator clips or solder I just used some pliers to bend a breadboard wire to it.
   ![[IMG_5699.png|300]]
2. I also only had 220 Ohms resistors but as the Lab said all worked out fine.
3. Lastly for some reason pin 8 would not work coming off my ardino so I swapped to pin 12 in my code and all things worked.
     ![[IMG_5698.png|400]]


I did add a potentiometer to my set up to then control the pitch in a more structured way than the presser sensor.

#### The Servo.
I had alot of fun with this.
everything went smoothly.

![[IMG_5697.png|400]]

Still having the potentiometer on my board from the last lab I used it to move my servo.

I then used the pressure sensor. I had an issue that the senor was picking up phantom pressure so the servo would twich on its own:


![[pressure one.gif]]![[pressure two.gif]]

I fixed that with fine tuning the mapping in the code:

![[pressure two.gif]]

After that I made some code of my own that would make the servo wave for 3 time after I push a button.
![[Wave.gif]]

The code was really simple as it was just modified from Lab:

![[Wave Code.png]]

I made two variables so that I didn't have to copy paste the values as I tuned the time between the waves and the angle of the arms.

I was curious if there was a way to make a another loop within the "void loop"?

