---
layout: post
title: The Topography of Stephen Curry
image: /img/2015-08-03-The-Topography-of-Stephen-Curry.png
description: Created for a class called Sculpting Data into Everyday Objects, The Topography of Stephen Curry is a 3D-printed visualization of every shot attempted by Golden State Warriors point guard Stephen Curry during his 2014/15 MVP season.
---
Data collection and data analysis are both enormous parts of the modern professional sports industry. During every NBA basketball game, for example, cameras track and record the exact position of every player, plus the ball, 25 times per second. The result is several terabytes worth of X, Y, Z coordinates and an unprecedented level of insight into the nuances of professional basketball. The NBA, in partnership with STATS LLC., calls the system SportVU, and even after two full seasons of league-wide use it remains an absolutely staggering tool. This project is an attempt to visualize a tiny fraction of that data. 

<figure>
<a href="https://lh3.googleusercontent.com/CSGV_1WJU4E9aaTF_daZnFgaUopvXtE5pXuqXdXgZOA=w600-h310-no" data-lightbox="SportVU" data-title="A play animated using data collected by SportVU. <em>Source: NBA</em>">
<img src="https://lh3.googleusercontent.com/CSGV_1WJU4E9aaTF_daZnFgaUopvXtE5pXuqXdXgZOA=w600-h310-no" alt="Sample SportVU animation" title="A play animated using data collected by SportVU. Source: NBA"> 
</a>
<figcaption>A play animated using data collected by SportVU. <em>Source: NBA</em></figcaption>
</figure>

Created for a class called "Sculpting Data into Everyday Objects," <em>The Topography of Stephen Curry</em> is a 3D-printed visualization of every shot attempted by Golden State Warriors point guard Stephen Curry during his 2014/15 MVP season.<sup><a href="#fn1" id="ref1">1</a></sup> Starting by scraping the raw data from the Internet, then interpolating success rates at each point on the court, I produced a shooting "heat map," which was further used to algorithmically generate a computer-modeled basketball as though it were being selectively deflated in specific regions, essentially creating a topographical map of a basketball court, with elevation corresponding to shooting frequency and success rates from a given position. The final piece has been 3D-printed using ColorJet Printing technology to produce a life-size basketball in full color and detail.

For context, and for anyone reading this who doesn't follow basketball, Steph Curry's 2014/2015 season was almost impossibly great. Curry shot for a .487 field goal percentage including an outrageous .443 from beyond the 3-point arch. He smashed the previous NBA record for threes made in a single season<sup><a href="#fn2" id="ref2">2</a></sup> by 14, despite only playing in 80 of 82 games and sitting out 17 entire 4th quarters due to overwhelming leads. In short, he was almost preposterously excellent, and he produced a lot of exciting data.

<h3>Process</h3>

The NBA doesn't make raw SportVU data publicly available, but manually extracting the bits I wanted was fairly straightforward. I scraped my data from <a href="www.basketball-reference.com">Basketball Reference</a>, but the same process works using the NBA's own site.<sup><a href="#fn3" id="ref3">3</a></sup> 

<figure>
<a href="https://lh3.googleusercontent.com/fVvYytk1B86fBwK62A9p9zsyEf1bDw3innGB_9xWOF8=w1960-h1520-no" data-lightbox="Visualization1" data-title="My initial attempt at vizualizing the shooting data, using discrete data points instead of interpolated values.">
<img src="https://lh3.googleusercontent.com/fVvYytk1B86fBwK62A9p9zsyEf1bDw3innGB_9xWOF8=w1960-h1520-no" alt="Initial attempt to vizualize using discrete data points" title="My initial attempt at vizualizing the shooting data, using discrete data points instead of interpolated values.">
</a>
<figcaption>My initial attempt at vizualizing the discrete data points. Produced using Rhino Python.</figcaption>
</figure>

Above is my initial attempt at visualization. Early on, rather than a complete collection of all 1341 individual shot attempts, I borrowed a model from Peter Beshai's excellent <a href="http://peterbeshai.com/buckets/app/#/playerView/201939_2014"> Buckets app</a>, where data points are also scaled to reflect success rates from that position. In this model, which I created using a Rhino Python script, the height of each data point represents success rate relative to the league average from that position. 

The model itself looks sort of nifty, but the discrete data points aren't much good for 3D printing (or least they didn't match the image I had in my head), so I decided to try a new approach. In order to produce a model that I could better map onto the surface of a basketball, I took a cue from Kirk Goldsberry and created a heat map from the raw data. Programmed using Processing,<sup><a href="#fn4" id="ref4">4</a></sup> my heat map gave me continuous values for the entire surface area of the court, and better lends itself to creating the deflated basketball that I was imagining.

<figure>
<a href="https://lh3.googleusercontent.com/NcUcihDI1sxR0fzsiWRSnMbRogQDEx1sTN7FdenIrbA=w992-h984-no" data-lightbox="Heatmap" data-title="A animated visualization of my heat map generation.">
<img src="https://lh3.googleusercontent.com/NcUcihDI1sxR0fzsiWRSnMbRogQDEx1sTN7FdenIrbA=w992-h984-no" alt="Animated heat map generation" title="A animated visualization of my heat map generation.">
</a>
<figcaption>Generating a heat map in Processing.</figcaption>
</figure>

With the data formatted to my liking, I moved on to producing the three-dimensional basketball model. Working in Rhino, I produced the flat model that you see below, but didn't have much success working on spherical objects, so I had to look for an alternative solution in order to effectively deform a ball.

<figure>
<a href="https://lh3.googleusercontent.com/Kz5uRxc-oZbTLA0V2V4mjQecoyJycm65r1DJG5HHGE0=w1966-h1528-no" data-lightbox="3DHeatmap" data-title="A three-dimensional version of the heat map projected from a plane. Fun fact: Because of a typo, this model was actually made using data from Steph's 2013/14 season. Whoops!">
<img src="https://lh3.googleusercontent.com/Kz5uRxc-oZbTLA0V2V4mjQecoyJycm65r1DJG5HHGE0=w1966-h1528-no" alt="Three-dimensional heat map projected from a plane." title="A three-dimensional version of the heat map projected from a plane. Fun fact: Because of a typo, this model was actually made using data from Steph's 2013/14 season. Whoops!">
</a>
<figcaption>A three-dimensional version of the heat map projected from a plane. Very dense model. My computer wasn't thrilled.</figcaption>
</figure>

My priority was to create a model instantly recognizable as a basketball, as well as to create an illusion that the deformations on the ball's surface seemed natural (natural despite showcasing Steph Curry's stats, which don't look like the sort of of thing that occurs in nature). I needed a method that would maintain the original curvature of the ball's surface, meaning that the hottest areas on the heat map, the areas that would appear most fully inflated, would also be no higher than the natural surface of the ball if it were a normal sphere. I achieved my best results with  Mudbox, using my heat map as a displacement guide to produce the deformations.

<figure>
<a href="https://lh3.googleusercontent.com/HybPnO06wixBgOMHgVJWDT7ouzKvwxzaz6mkXZAXXQY=w2116-h1358-no" data-lightbox="DeformedSphere" data-title="The deformed sphere, produced in Mudbox.">
<img src="https://lh3.googleusercontent.com/HybPnO06wixBgOMHgVJWDT7ouzKvwxzaz6mkXZAXXQY=w2116-h1358-no" alt="The deformed sphere, produced in Mudbox" title="The deformed sphere, produced in Mudbox.">
</a>
<figcaption>The deformed sphere, produced in Mudbox.</figcaption>
</figure>

With the data in good shape, I moved on to making my model actually look like a basketball (as opposed to a Rorschach emoji). The exterior of a basketball consists of eight pebbled leather panels, divided by thick black rubber seams, so I began by adding the seams.

<figure>
<a href="https://lh3.googleusercontent.com/Mu2zgzK-JTja71w2MNi7AbMM6z0BCPM5lTly4t2YQKM=w1962-h1524-no" data-lightbox="Seams" data-title="Adding the seams between the basketball's panels, using Rhino.">
<img src="https://lh3.googleusercontent.com/Mu2zgzK-JTja71w2MNi7AbMM6z0BCPM5lTly4t2YQKM=w1962-h1524-no" alt="Adding the seams between the basketball's panels." title="Adding the seams between the basketball's panels, using Rhino.">
</a>
<figcaption>Adding the seams between the basketball's panels, using Rhino.</figcaption>
</figure>

Next, I created the pebbled leather texture on the surface of the ball. It's pretty straightforward to fake that effect using a bump map, but I was designing with 3D printing in mind, and bump mapping is no good in a physical object, so I had to take the more complex route.<sup><a href="#fn5" id="ref5">5</a></sup> Using Mudbox and working one panel at a time, I sculpted the leathery texture onto the ball by actually displacing the surface.

<figure>
<a href="https://lh3.googleusercontent.com/GcyH-9AYWOcHcsbgtNCODxsJPfOYLXAyNej9kHizQ-I=w780-h430-no" data-lightbox="Texture" data-title="Sculpting the leathery texture onto the ball using Mudbox.">
<img src="https://lh3.googleusercontent.com/GcyH-9AYWOcHcsbgtNCODxsJPfOYLXAyNej9kHizQ-I=w780-h430-no" alt="Sculpting the leathery texture onto the ball using Mudbox." title="Sculpting the leathery texture onto the ball using Mudbox.">
</a>
<figcaption>Sculpting the leathery texture onto the ball using Mudbox.</figcaption>
</figure>

With the texture in place, I could finally start printing actual objects. Below is a trial print in ABS plastic. It's three inches in diameter (about 31% of a real basketball's 9.55 inch diameter), which wound up being too small to get any discernable detail in the surface texture.

<figure>
<a href="https://lh3.googleusercontent.com/4uWzxgR_2-nHQviOWVDLPB6pDhMB3VQxtjzvitWqpVk=w2148-h1610-no" data-lightbox="ABSball" data-title="The final design printed in ABS plastic at 31% scale.">
<img src="https://lh3.googleusercontent.com/4uWzxgR_2-nHQviOWVDLPB6pDhMB3VQxtjzvitWqpVk=w2148-h1610-no" alt="Ball printed in ABS plastic at 31% scale." title="Model printed in ABS plastic at 31% scale.">
</a>
<figcaption>Basketball in ABS plastic at 31% scale. Printed using a Stratasys Fortus 250mc.</figcaption>
</figure>

The ABS model was printed on a Stratasys Fortus 250mc, which prints using a method called Fused Deposition Modeling (FDM). If you've ever seen a MakerBot work then you're familiar with FDM printing; FDM printers work by extruding a thin molten filament along tightly defined paths to form layers that build up the model. For many people, FDM is basically synonymous with 3D printing, but it's actually just one of a wide range of fabrication techniques, and in order to print my final model at life scale, I switched to a different printing technology.

As the final step before printing the real thing, I digitally painted the model to look like a basketball.

<figure>
<a href="https://lh3.googleusercontent.com/2E8RjKc2Kl-6UPuawPQQ2sGHxkf7Yckk3RU_YRxIgHE=w1000-h643-no" data-lightbox="Painted model" data-title="A full-color rendering of the finished product. Painted using ZBrush.">
	<img src="https://lh3.googleusercontent.com/2E8RjKc2Kl-6UPuawPQQ2sGHxkf7Yckk3RU_YRxIgHE=w1000-h643-no" alt="Full-color rendering" title="A full-color rendering of the finished product. Painted using ZBrush.">
</a>
<figcaption>A full-color rendering of the finished product. Painted using ZBrush.</figcaption>
</figure>

In powder-bed or ColorJet Printing (CJP), the machine prints by spreading a thin layer of a powderized printing material over the entire surface of the print bed. Once the powder is spread, a print head spreads a liquid binding agent over the cross-sectional area of the layer, hardening the material and fusing it to the layers beneath. Another layer of power is then spread on top, and the process repeats. In addition to generally being faster and cheaper than FDM printing, by mixing traditional printer ink with the binding agent, powder printers are able to print in the full CMYK color spectrum (up to 6 million colors). My final, lifesize model was printed using a Z Corp ZPrint 650.<sup><a href="#fn6" id="ref6">6</a></sup>

<figure>
<a href="https://lh3.googleusercontent.com/MF6EJoAe6mN7cu8gy_Iz_tFwGYrxwGaz0NbfaEsjF6s=w2148-h1610-no" data-lightbox="Final1" data-title="The final, lifesize print. Produced on a Z Corp ZPrint 650.">
<img src="https://lh3.googleusercontent.com/MF6EJoAe6mN7cu8gy_Iz_tFwGYrxwGaz0NbfaEsjF6s=w2148-h1610-no" alt="The final, lifesize print." title="The final, lifesize print. Produced on a Z Corp ZPrint 650.">
</a>
<figcaption>The final, lifesize print. Produced on a Z Corp ZPrint 650.</figcaption>
</figure>

The end result from a powder print like this is essentially a piece of ceramic,<sup><a href="#fn7" id="fn7">7</a></sup> but in the interest of making the finished piece feel as much like a real basketball as possible, I applied a thin coating of soft-touch rubber to the surface. Combined with the pebbled leather, it's actually a pretty good grip, and it has a familiar hand feel.

Here are a few more angles of the finished product.

<a href="https://lh3.googleusercontent.com/HPOMkIzeimdbS6HbqFLrJMIMH49dUgcjMrlbxk8YsLU=w1000-h664-no" data-lightbox="Final2">
	<img src="https://lh3.googleusercontent.com/HPOMkIzeimdbS6HbqFLrJMIMH49dUgcjMrlbxk8YsLU=w1000-h664-no" alt="Finished product 2" title="Finished product, 2">
</a>

<a href="https://lh3.googleusercontent.com/J-QfSFCzAZRvTXTFTt8RImlhlbg-vfB5BLY8ne6g_5A=w1000-h664-no" data-lightbox="Final3">
	<img src="https://lh3.googleusercontent.com/J-QfSFCzAZRvTXTFTt8RImlhlbg-vfB5BLY8ne6g_5A=w1000-h664-no" alt="Finished product 3" title="Finished product, 3">
</a>

<a href="https://lh3.googleusercontent.com/dKP4JHRhb8JMGah-OJQvJcX_1KZe3slPVJdtMVMDWfg=w1000-h664-no" data-lightbox="Final4">
	<img src="https://lh3.googleusercontent.com/dKP4JHRhb8JMGah-OJQvJcX_1KZe3slPVJdtMVMDWfg=w1000-h664-no" alt="Finished product 4" title="Finished product, 4">
</a>

<a href="https://lh3.googleusercontent.com/hHlLphuULjXLnrmJupI0iSYCqpn6HVLpiGxKUpRbivw=w1000-h664-no" data-lightbox="Final5">
	<img src="https://lh3.googleusercontent.com/hHlLphuULjXLnrmJupI0iSYCqpn6HVLpiGxKUpRbivw=w1000-h664-no" alt="Finished product 5" title="Finished product, 5">
</a>

<h3>Final Thoughts</h3>
I'm a tactile learner, so throughout this project I was excited by the prospect of being able to hold the data in my hands. As it stands, a model like this isn't hugely useful in terms of analytics, but to me at least, the tangible element is very compelling.

During the early stages of this project, I didn't focus exclusively on Steph Curry. I made test models with data from other players, including James Harden, LeBron James, Russell Westbrook, and Anthony Davis. Printing multiple basketballs became too cost prohibitive, so I narrowed my focus to Curry. Every player on that list plays a radically different game, with correspondingly different shot charts, so the maps that I produced varied dramatically. Blown up large and then stamped onto the face of a basketball, the map is a little bit larger than my palm; about the size of, say, an NBA player's palm instead. There are lots of interesting roads to follow in order to make a genuinely useful analytical tool from all this, but for now the impression of the map creates a unique handprint for the season. In Curry's case, an historically great one.

<br>
<hr>
<div class="footnotes">
<ol>
<div id="fn1"><li>Although Golden State played an additional 21 playoff games during their title run, due to time constraints I’ve only included data from regular season games.<a href="#ref1" title="Jump back to footnote 1 in the text.">&#x21A9;</a></li></div>

<div id="fn2"><li>Previous record holder: Stephen Curry<a href="#ref2" title="Jump back to footnote 2 in the text.">&#x21A9;</a></li></div>

<div id="fn3"><li>I'm not going to get into my scraping code here mainly because this post is about visualizations, but also because my Python is fairly sloppy. If you're interested in web scraping, <a href="http://www.gregreda.com/2015/02/15/web-scraping-finding-the-api/">Greg Reda</a> has some excellent tips.<a href="#ref3" title="Jump back to footnote 3 in the text.">&#x21A9;</a></li></div>

<div id="fn4"><li>My heat mapping code is forked from Justin Dailey's <a href="http://www.openprocessing.org/sketch/46554">Heat Distribution</a> system.<a href="#ref4" title="Jump back to footnote 4 in the text.">&#x21A9;</a></li></div>

<div id="fn5"><li>Bump mapping uses simulated light to distress a rendered surface and produce the illusion of a realistic surface. It does not, however, actually modify the surface, so it's not very helpful when 3D printing.<a href="#ref5" title="Jump back to footnote 5 in the text.">&#x21A9;</a></li></div>

<div id="fn6"><li>Z Corp was acquired by 3D Systems in 2012.<a href="#ref6" title="Jump back to footnote 6 in the text.">&#x21A9;</a></li></div>

<div id="fn7"><li>Apologies to anyone hoping to try dribbling with this.<a href="#fn7" title="Jump back to footnote 7 in the text.">&#x21a9;</a></li></div>

</ol>
</div>
