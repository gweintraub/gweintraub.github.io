---
layout: post
title: Visualizing NYC (And Some Mutilated Animals)
description: Assignment for Data Visualization From 2D To 4D
---

In December, 2014, following a Staten Island grand jury's decision not to indict the officer who killed Eric Garner, as well as the murder of two NYPD officers in BedStuy shortly thereafter, police across the city engaged in what appeared to be a virtual work stoppage, with citations issued and summonses for minor offenses fell by nearly 94% from the previous year. I took a look at some of that data in order to experiment with D3js.

Using the Socrata Open Data API to sift through NYC Open Data, I collected parking violations issued after December 1. Parking citations also include details about the vehicle, and I was curious about patterns relating to the brands involved, so I further filtered the data to exclude entries with no vehicle make entry (looking at the unfiltered data, these were relatively uncommon). My final query was:

`https://data.cityofnewyork.us/resource/c284-tqph.csv?$where=issue_date >= '2014-12-01T00:00:00' AND vehicle_make IS NOT NULL`

Ultimately, I had some trouble using D3 with the vehicle makes, so I held off on visualizing the vehicle information and just made a chart illustrating violations cited based on days of the week. It tells us very little about post-Eric Garner policing, but I used the Mets' colors, which just felt right.

<iframe width="100%" height="300" src="//jsfiddle.net/xyeu4b66/1/embedded/result/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

***

Largely unrelated: There's a fairly distressing dataset available of animals found decapitated across the city. Using <a href="https://batchgeo.com/">BatchGeo</a> I mapped out their locations and included the grisly data. Somewhat disappointingly, they didn't form a giant pentagram or anything. I expected better from New York's cultists.

<p><iframe src="//batchgeo.com/map/aecd4fe751fea9cf3aaf5ca70c4a4147" frameborder="0" width="100%" height="550" style="border:1px solid #aaa;"></iframe></p><p><small>View <a href="https://batchgeo.com/map/aecd4fe751fea9cf3aaf5ca70c4a4147">Decapitated Animals</a> in a full screen map</small></p>