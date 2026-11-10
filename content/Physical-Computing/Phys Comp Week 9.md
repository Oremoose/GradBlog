---
title: Physical Computing Week 9
draft: false
tags:
  - ClassNotes
  - Physical-Computing
  - FinalProject
---
## Class Notes:
When Debugging remember to double check the source references:
https://developer.mozilla.org/en-US/


## Homework 
For my final I have decided to make a Simon game

![[SimonGame.png|250]]

with my fidget toy.

I ordered more solenoids and a driver for them and while I am waiting I jumped ahead to next weeks labs because I wanted to be confident in my ability to properly power my final before I got too ahead of my self. 

I already had a [28BYJ-48 – 5V Stepper Motor](https://components101.com/sites/default/files/component_datasheet/28byj48-step-motor-datasheet.pdf) with a [ULN2003 Driver Board](https://www.hadex.cz/spec/m513.pdf) I got it powered using a 10v plug from my partners desk lamp.

While following the lab I had an issue of my board not connecting to my computer when ever I had the 10v plugged in. Turned out that I had accidentally swapped the power and ground wire coming from the DC power jack, I meant for Red to be power and White to be ground, once I swapped them back around proper everything went Smooth.

The motor seemed slow and stuttery I think that it was because the compositor that I used was only rated for 10mf and I should grab a beefer one from the shop when I am there next. I also tested some examples using the Stepper.h library one of which was written by tom igo himself. 