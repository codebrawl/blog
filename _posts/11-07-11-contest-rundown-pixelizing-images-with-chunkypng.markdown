---
layout: article
title: "Contest rundown: Pixelizing images with ChunkyPNG"
---

<style>
  #main img{
    float: right;
  width: 30%;
    margin: 0 0 10px 10px;
  }
</style>

See? I told you [ChunkyPNG](https://github.com/wvanbergen/chunky_png) was a fun library to play around with? Our [second contest](http://codebrawl.com/contests/pixelizing-images-with-chunkypng) challenged the contestants to pixelize an image of a tapir and it had 45 entries. I'll just cover the top 5, starting with the winning entry by Inge and taking you through the rest of the smart, small and crazy solutions. Let's go!

![Inge Jørgensen's and Roger Braun's result images](https://gist.github.com/raw/71598aeb1d823c9229ac/7a3f3df14f8d2e8c9f179126cb9b76685525f7c3/output.png) [Inge Jørgensen](http://codebrawl.com/users/elektronaut)'s [implementation](http://codebrawl.com/contests/pixelizing-images-with-chunkypng#elektronaut) is solid, he uses the average color of the pixels within blocks of ten by ten pixels, giving the end result a smooth look. His ten line solution is a little concise for my taste, making the code a bit more difficult to understand at first glance. Congratulations for taking the first place!

[Roger Braun](http://codebrawl.com/users/rogerbraun)'s resulting image is _exactly_ the same as Inge's and [his way of solving the problem](http://codebrawl.com/contests/pixelizing-images-with-chunkypng#rogerbraun) is comparable, although quite a bit longer. Roger ended in second place by splitting the whole thing up in focussed methods and adding `ChunkyPNG::Color.average`, to calculate the average color. I prefer this over shorter implementations, because the code is more readable and can be reused -- and turned into a ChunkyPNG extension -- more easily.

![Chris Thorn's result image](https://gist.github.com/raw/233cae774314821d4a74/4e7ec69a2ba2a20ec3cd93dfdc1aa63ee9f21dc2/warhol.png)
Taking the bronze, [Chris Thorn](http://codebrawl.com/users/thorncp) has the same result image too, and also extends the ChunkyPNG library nicely. [His implementation](http://codebrawl.com/contests/pixelizing-images-with-chunkypng#thorncp) is almost twice as long as Roger's, but that's probably because he added `ChunkyPNG::Image#pixelize_with_warhol!`, which gives you an interpretation of the pixelated output inspired by Andy Warhol's work. Nice touch.

![Ian Terrell's result image](https://gist.github.com/raw/773a54c35f957b90194c/398e3d0e863d0be1cb0954574423321bb813cf58/gbr.png)
[Ian Terrell](http://codebrawl.com/users/ianterrell) was the first one to submit [his entry](http://codebrawl.com/contests/pixelizing-images-with-chunkypng#ianterrell) and I can hardly imagine he didn't do this work before the contest started. He takes the fourth place by showing us _eleven_ ways to pixelate an image, using the average color like the other contestants, taking the darkest color, shuffeling the colors around and so on. Be sure to check out the result images, there are some great ones in there. His entry is split up into eleven files and there's a lot of duplication, while it feels like most of it could be put into ChunkyPNG by extending it. Besides that, amazing work!

![Will Leinweber's result image](https://gist.github.com/raw/1050731/7fe1eeb3d931db37595abd57d8ec4c0f5f8a3685/8bit.png)
[Will Leinweber](http://codebrawl.com/users/will) took it one step further and thought "Ten by ten pixles? Might as well go 8 bit while we are at it.". His [entry](http://codebrawl.com/contests/pixelizing-images-with-chunkypng#will) plays around with the colors, creating two 4-bit images and one 8-bit one. Somebody needs to build a originality prize feature, so we can give it to Will. A well-deserved 5th place.

Thanks to everyone for entering this week and thanks for everyone who voted, it was quite the task. Willem van Bergen (the creator of ChunkyPNG) recently started a library named [ChunkyBits](https://github.com/wvanbergen/chunky_bits), which is a ChunkyPNG image processing algorithms extension. He really wants to have a pixelate method in there, so it would be awesome if the contestants could write a patch to implement that.
