---
title: Example Title
draft: false
tags:
  - Homework
  - ICM
  - p5js
---
 [My Sketch](https://editor.p5js.org/Oremoose/sketches/I4K-vDynu)
# This Project is Described in 3 Words:
1. Simple
2. Cubism
3. entropy

This Project was inspired in part of the Cubist movement and their desire to depict their subjects in multiple dimensions. This is something I paralleled in my Untitled thesis work for my undergrad at Towson University. In which I used a Projection mapping and a lot of editing in Photoshop to make a portrait of a classmate appear in  three dimensions.
This time I wanted to the opposite. 

1. I wanted take out the complex photo manipulation of major photo editors where I only needed 4 angles. Making it simple and easy to set up and execute.

2. Ultimately I want the final work to share that Cubistic aesthetic of showing multiple perspectives at once. Even to the point of having Multiple people joining in to the point of deterioration.

3. The reason that I wanted to make the end of the piece end in entropy is because there was a saying, "Everything lives forever on the Internet". That unfortunately is not true, See the death of the Space Jam website. I wanted my work to lean into that. 

# How it was done
## 1. Initial Idea
Playing about with the `loadPixels()` 
I figured that while I can select pixels and then drop the Alpha channel to zero I can so that images behind the image being edited. This can be see here [Cubism Test](https://editor.p5js.org/Oremoose/sketches/r57R-W2CG). which was inspired by the work sheet from the other week. 

I then wanted to have it so that as more streams were add the gap between the lines of visible pixels would widen and so more layers can be seen at once to absurdum.

## 2. Failure
I attempted this with live stream captures but due to lack of knowledge I could not seem to be able to load and manipulate the pixels that I wanted.

## 3. Pivot
 Pivoting to try it with still images. I had 4 images taken of my head:
 ![[Screenshot 2025-11-02 172116.png]]

took the images into photoshop to make sure they were all aligned equally and then Cropped so that all the images were exactly the same shape.
![[Screenshot 2025-11-02 171910.png]]

From there I added them to p5.sj and began to code.

I had made a function in my test I was hoping to sue throughout this project:
```js
function cube(name, n, i) {
  image(name, 0, 0, windowWidth, windowHeight);
  name.loadPixels();
  for (pix = n; pix < name.pixels.length; pix += i) {
    name.pixels[pix + 3] = 0;
  }
  name.updatePixels();
}
```
It was clean and was portable.
*I particularly like the part where I single out just the Alpha channel in the Pixel array*

While this worked really well in my test once I added third image I needed to increase both the number pixels I skip over and the pixels that I need to edit.

So alas my little Function was not used.

## The decay of it all
A quick explanation of the Code. 
In the Draw function I use `millis() / 1000;` to get an even count of the passing of time.
Then an accordion list of Functions that are filtered through If statements that would trigger each function every 10 secs aside from the last two that go out in 5.

In the second half of the If statements thing go awry as the images leaves the background begins to bleed through. This happens, I am assuming, because when the pixel arrays are updated the pixels that are turned off are actually deleted and so the don't line up properly and the whole image is lost. 

I really liked this ending as I could not just continue to increase the amount of streams that exist in the canvas to evoke the unraveling insanity I originally wanted. The Data more or less eating itself is that entropy that all things on the Internet will eventually get to.