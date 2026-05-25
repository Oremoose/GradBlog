---
title: AR Modalities Week 3
draft: false
tags:
  - ClassNotes
  - AugmentedReality
  - ImageTracking
---
## Class Notes:
### Look up:
- Orthographic Camera - [documentation site](https://developers.snap.com/lens-studio/lens-studio-workflow/scene-set-up/camera#orthographic-camera)

### Image Tracking
- Can be seen as the OG modality due to the fact that is a 1:1 pattern recognition.
- The best image is complex and highly textured, and has contrasting elements
- matte images work better than glossy type.
- IF images are really recognizable (say the bicycle version of the queen of spades), the instance will appear on all queen of spades regardless of where it is.

### Publishing Filters

Tween manager must stay at the top of the hierarchy.



## Homework 

### Intro
I Wanted to make a double sided experience.
I thought it could be cool for like a business card or a post card that could come to life.
Basically I thought of a 2D object has an different experience on each side of the Objects.

I landed on a doing something with a Pokémon card because Pokémon Go is turning 10. So I thought it would be a nice tribute to make a Pokémon AR experience.

Looking online i found an [fbx Bulbasaur!](https://free3d.com/3d-model/bulbasaur-pokemon-57218.html?dd_referrer=) By a user aptly named poke_master.

Sadly, I no longer own any of my OG Pokémon cards (I gave them all to my younger brother).
I set out to make my own. 
I took the front from a listing on [TCGplayer](https://www.tcgplayer.com/product/107041/pokemon-base-set-shadowless-bulbasaur?country=US&utm_campaign=20451986774&utm_source=google&utm_medium=cpc&utm_content=&utm_term=&adgroupid=&gad_source=1&gad_campaignid=20451985907&gbraid=0AAAAADHLWY1NpS6sjlh5pte_PnC1F1Aoy&gclid=CjwKCAjw1tLOBhAMEiwAiPkRHuFy6qTaA7MvnRmJFpZGvwp37o5P7BlV0b72r2Dd1NFA1deTZ_a8vhoC3FAQAvD_BwE&Language=English)and the back I attainted from [AtomicmonkeyTCG](https://www.deviantart.com/atomicmonkeytcg)on Deviantart.

### Making the Card
I attempted and failed at double siding printing my card.

![[IMG_4335-1.png]]

The Cards on the left were attempts one and two. the alignment of the front and back so when I trimmed the cards is sliced either the front or back really badly.

The solution was to print the front and back separately and then glued them together and then trimmed them. But even then the cad came out really janky. 

### The Idea 
Once I Had the card made I was not 100% sure what I wanted to do.
I hade the Bulbasaur card and model. I know that I could put the Bulbasaur on the card which is cool. But I wasn't sure what to put on the back because it would be something that would trigger no matter what Pokémon card you had. 
Then I remembered the bumpers on during the commercial breaks of the show when you had to guess "Who's that Pokémon?".

### Putting it all together
So that is what I did. [I found the clip online](https://www.youtube.com/watch?v=JtM4p0phtio) and took it into premiere stripped the audio to its own track and then output the frames as a png sequence and moved on to Lens Studio.

![[Screenshot 2026-04-08 230416.png]]
I just followed the tutorial as needed to refresh my memory for the spots i was shaky on.

In the end this is what I got:

<iframe width="560" height="315" src="https://www.youtube.com/embed/lebnyiL21kk?si=0eMJ5MCm0c7rgLvK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Conclusion

Things that I need to work on:
- modifying textures of materials in Lens Studio. I dont think I fully get it so Baulbasaur isnt looking as clean as he should. The Model came will all the needed color files but I could not fix his eyes.
- the model also came ready for animation and I did not try that even though i think it would be great.

What the next step :
- Make the filter hold more cards with different Pokémon
- reach out to Pokémon and have them add this to one of there apps.