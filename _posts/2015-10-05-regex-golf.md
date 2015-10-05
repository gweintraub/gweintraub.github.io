---
layout: post
title: Regex Golf Needs More Rules
description: The regex is hard. But the interface is harder.
img: https://imgs.xkcd.com/comics/regex_golf.png
---

The only real rules provided for <a href="https://regex.alf.nu/">Regex Golf</a> are "Type a regex in the box. You get ten points per match (or lose ten, if you match something you shouldn't); each character costs one point." That seems fairly straight forward, until suddenly it isn't. 

The first challenge while golfing is to determine the patern itself. That's a non-trivial task in its own right, and the game even admits that it's being pretty vauge about it all (the fourth level says "Not really clear what you're supposed to do here"). Obviously the game should be hard, but having to sniff out the pattern is something of a distraction since in most cases you write regex for patterns you already know. Whatever though. We're coding. Finding patterns is fun.

My bigger confusion is how the scoring is implemented, and how the game indicates incorrect matches. I'm not a regex ninja yet, but I'll enter an expression that seems correct and gives me lots of green checkmarks and seems ostensibly right, but leaves with a negative score (an impossibly excellent score in real golf, but pretty lousy in regex). Also, what are the underlined sections supposed to tell me? No one knows.

<img src="https://lh3.googleusercontent.com/ywBAMg-OM7x12ruBQxNpVWIlWKdK7mSRRKpbo6MEZCGk3lydLO_u_BWJNq02mg9fUwdlONFSdr3OM-mJsv9zwC6RtKEP6p2CylAZRYuXKmvjweA8YibafIBqf8KJ0tqnEX6nRgO4TppKcflOCTCf2OTUyX1S0WsX74nPhcMraGd-zoB-BdZepgqIjXQWp_b1mx_HJUBpMtOnF5HDjBMYzGGHmZAKoe40o0lUgcWLW7Jkkz1abAnyVUYU8nzHc1wPbSzknwqv3Gg6O1ze1qr7VlzniNs-i5kNqCBLKP03I8dnd7DnblTn1SSMNt9ooWOy1yEocfeSl4w3GvpYav5gSe64hXYFRLRqY-6L3YRM-6YyS4nLLM0PtLZURHTqyPnoK-y2OEsOeUwbsihfs6BdHqTpSuY_2NrH1LREuoY39dhTh14ijXrnSg0oU-RNA6H92grOn5UrpttXVgWIwVQtUHs2ftqfcu16LbGmYmX9yBTAJbRyBVnmWlIgxBqt-k4TVg-ldlL1aLU0ygzrh1VXfzu0erxzRuBwqSqogZ4gWP4=w2160-h1216-no" alt="Regex Golf" title="Regex Golf">

I'm not good at real golf either, but at least a sand trap always looks like a sand trap.