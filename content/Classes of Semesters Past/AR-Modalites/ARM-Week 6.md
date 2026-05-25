---
title: AR Modalities Week 6
draft: false
tags:
  - ClassNotes
  - AugmentedReality
  - LensStudio
---
## Class Notes:
Custom Object tracking:
One way to recognize custom Object is through machine learning.
Machine learning start with Object recognition and then goes into...


All of this is built on a 2D view of the world looking at through the camera as a flat image.

You can use building as trigger 



## Homework 

Final project: Star wars day

With May 4th, a.k.a. May the forth be with you, a.k.a Starwars day. I decided to make a filter commemorating the classic scene from "A New Hope" when Obiwan uses his Jedi mind ticks to convince the Storm troopers that R2 and C3P0 were not the droids that they were looking for.

## The Plan:
Make a filter that has C3P0 and R2D2 over the shoulder of the person and when the person waves their hand the and voice line "These are not the Droids you are looking for" and then R2D2 and 3CP0 have disguises appear on them.

The Bots:
![[R2-D2.png | 200]]![[c3po.png |200]]


The disguises:
![[R2-D2-disguise.png | 200]]![[c3po-disguse.png |200]]


I began with simply triggering the behavior with a simple raise of the eyebrows.

![[EyeBrows.gif]]

I then attempted to be ambitious to trigger the behavior based on a distance check of my hands to the opposite shoulder. So that by waving my hand like obiwan did the effect will happen.
But like with a few weeks ago the body tracking requires that you be farther from the camera than I wanted.

After looking through the Lens Studio Documentation I came across the [hand tracking gestures](https://developers.snap.com/lens-studio/features/ar-tracking/hand/hand-gestures#overview) that allow triggers based on a few basic hand signs. One of the hand signs that can be used is a simple open palm. which I realized that is all I need. After writing a custom script and adding the audio file the filter was ready to ship.

<iframe width="560" height="315" src="https://www.youtube.com/embed/p9Hky6TTG4A?si=z_9z7_GMEeL1sTG9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

While yes, that means that if someone simply raises their hand then the filter will work. However I think that with the notion that the person is aware of the scene from Starwars and the jedi mind trick wave. The user will naturally want to wave with an open hand so I am not too worried about it.

![[Pasted image 20260429211034.png]]
