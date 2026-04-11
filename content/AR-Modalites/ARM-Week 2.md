---
title: AR Modalities Week 2
draft: false
tags:
  - ClassNotes
  - AugmentedReality
  - Splatting
  - LensStudio
---
## Class Notes:
### Face Computer Vision
Detection - Identifying something as a face

##### How it works
1. Feature based
	1. looking for low level features eye/ face edges/ lips etc.
2. image based
	1. comparing images to a knowledgebase

Tracking 
Optical Flow Based tracking.
landmark (land point) points from the face that can be compared to how it moved

Recognition
machine learning is used to differentiate between face


head binding is need to for face filters to work
## Homework 

Remember to use the documentation.
fbx for 3d Objects

I am sorry but I failed to follow the assignment as given, I did not take an adjective and make a filter based on that word. If I did I hope I could get the word "appropriate" not the adjective though; the verb.

>APPROPRIATE *verb*
> ap·​pro·​pri·​ate ə-ˈprō-prē-ˌāt
>
>**:** to set apart for or assign to a particular purpose or use
>
>*appropriate money for a research program*
> 
>- [merriam-webster](https://www.merriam-webster.com/dictionary/appropriate)

The reason for this is that I already had an idea from the beginning of class.
Over spring break I went to the Whitney's Biennial.
 I saw an art piece, an inflatable by Pat Oleszko, that I liked and so I "stole" it.
 
 ![[IMG_4224.png | 400]]
 
 
 And by stole I mean that I took a very intentional video of the work so that I can make a Gaussian splat from it. (for more info on that look at my blog posts from [[New Portraits]])
 ![[MakingTheWhitneySplat.gif | 100000]]
 
When I made the splat I knew that the file could be quite light weight so that I could possibly fit it into a filter. and after the demo in the class I knew it was possible and so I went to make it happen.

So I cleaned up the splat and moved it into Lens Studio.
Lens Studio recognized the ply file as a splat and so I bound it to the face and scaled it to the point that it encompassed the whole head.

![[IMG_4293.jpg | 400]]

There was one issue the horn took up a lot of space.

![[Face Test one.gif]]

So i did made a second one with a cropped horn
![[Cropped horn.png]]

But I didn't like how it made it seem like some thing was missing.

So I kept the original and then added the kiss face gesture to toggle the head on and off because that was the closest to the face that clown was using.

![[Face filter test 2.gif]]

The trigger didn't work as consistently as i wanted.
But I think that is a snapchat issue not me.

### Reading:
https://www.vice.com/en/article/is-animating-dead-relatives-with-ai-cathartic-or-creepy-yes/

It may be because I have yet to lose an immediate family member. I found Deep Nostalgia unimpressive and I don't think that I would have any emotion attached to a poorly reanimated image.