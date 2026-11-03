---
title: Physical Computing Week 8 Midterm Reflection
draft: false
tags:
  - ClassNotes
  - Physical-Computing
  - Midterm
---
## Class Notes:
"What ever computer has better horse power is better at listening"

https://www.asciitable.com/

Remember that you can only use one port at a time. So when switching from the IDE to p5.js you need to close monitor of port from one so that the other can read from it.
## Homework 

### Midterm Reflection
The over all conception to finish the project I understand. The part that I wasn't 100% on how the code sent a sting via BLE to my phone. In the "Light blue" app I can choose how the phone interpreted the signal coming from the Arduino. Madina had Claude help us with some of the code and I forgot to get a copy of it from her, But once I do I am sure that I can figure it all out.

### Labs:
I caught up on the week 7 Labs:
#### Lab: Intro to Asynchronous Serial Communications
I got it all working well like we covered in class. However I was trying to read the potentiamiter from my Terminal using WSL like in the lab but WSL kept crashing and for the sake of time I moved on, but want to return and figure out why it keeps crashing automatically.


#### Lab: Serial Input to p5.js Using the p5.webserial Library
I got the 

Week 8 Lab:
#### Lab: Two-Way (Duplex) Serial Communication Using An Arduino and the p5.webserial Library

Here is my Sketch:
https://editor.p5js.org/Oremoose/sketches/RAgaoQt_m

I made a fairly simple sketch of a bouncing with 3 potentiometers and a button coming in to control the color of the ball and then direction of the bouncing. I did use the Chrome extension known as Shiffbot to help me dust off my p5.js knowledge.

<iframe width="405" height="720" src="https://www.youtube.com/embed/VJ_RgukilPA?si=Tc7BZbudRKE38_av" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


I had some hiccoughs along the way:

Issue 1:
I had to manually set the p5.js sketch to 1.4.0 for the sketch to work the function: "split()" is not part of the current p5.js library. 

Issue 2:
Once I had the code running the sketch would freeze after a 30ish seconds.
I think it was a buffer was still getting over whelmed by the amount of data coming from the Arduino. I tried getting some help from the Shiffbot and added a 50 millisecond delay on the end of the void loop. But it still gets jammed, I think one of my potentiometer is also coming loose from the breadboard




