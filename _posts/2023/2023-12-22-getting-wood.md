---
title: Getting Wood
---

I really thought that making wooden planks in Blender was going to be easy, just sculpt a little woodgrain into a box and it's good to go. It really turned out to be more complicated than I could have expected. I should clarify I am talking about sculpting planks for the purpose of 3d printing, specifically for some Wild West buildings I need for playing tabletop games - meaning the texture has to be in the mesh and exaggerated enough to be painted easily, so most of the tutorials I found were not super helpful for it.

![Wooden Textures](\images\posts\2023\wood-planks.png)

<!-- more -->

## Things that didn't work

I'm talking about this because I want to remind myself that learning how "not" to do something is not wasted time...

The first thing I tried was poly modelling planks. This is a super time consuming way to do things and really hard to get the roughness and irregularity of rough wood grain. It does give the best flexibility for slightly warping the boards and having split edges. But ultimately I had to try other things.

If I am not poly modelling then I guess I can try using the displace modifier and creating some texture that works as wood grain. This actually worked a little, but the lack of control over the texture was the real problem, resulting in very even grain that also just wasn't very realistic. Definitely getting closer though.

Sculpting! I tried modelling up a single plank then directly trying to sculpt the detail on using the draw sharp brush, or the crease brush, or something similar. Again this was super time consuming but the results were occassionaly pretty solid. Again it was hard to get the grain looking "just right".

## My final method

So I figured sculpting was right. What I did find was that I could get some rough wood grain alpha textures online and use these in the sharp brush to texture the wood. After that I could go back in and modify the wood as I needed. I eventually modified a few of the grain textures I found to exaggerate some deeper cuts for the benefit of being printable. A little warping of the planks and scraping the edges and it looked pretty good.

Building the houses then came down to layering these planks onto a simple box and just merging everything. I really had to decimate everything to keep the face count down because it could quickly grow to 10+ million for a single object. I hate losing the printable detail though.

![Wooden Textures](\images\posts\2023\wood-texturing.png)

## Making improvements

Well there's a lot to do here to improve this, mostly in designing a more interesting building (there is a decorative front not shown here), maybe breaking up the box a little more. I will need to print it and see how it paints before making any further decisions.

As for the wood grain, I think I might have more success using masks, something I've only just started figuring out, and then a mesh filter to inflate in a specific direction. I need to try some other things for a bit now though.

- Callum
