---
layout: post
title: The Winds of WinterBot\: Because Someone Has To Write It
image: 
description: 
---

George R. R. Martin began writing his <em>A Song of Ice and Fire</em> series in 1991. To date he has published five of a promised seven (and threatened eight) books, most recently <em>A Dance With Dragons</em> which was published in July of 2011. His next installment, <em>The Winds of Winter</em> has no known publication date. In the meantime, HBO's televised adaption of the series, <em>Game of Thrones</em> has outpaced Martin, leaving the show's writers to essentially make up their own version of what happens next in the series.

Unfortunately, HBO's writers have not produced exemplary content so far. Martin himself, while supposedly hard at work, has continued to produce blog posts about the foibles of the New York Jets, and has provided no updates as to the status of TWOW.

With millions of fans eagerly anticipating it's release (and a spot assured on all the relevant best-seller list), it's clear that someone needs to write this damn book. That someone, I've decided, will be a Twitter bot. It can't be worse than what HBO's working on.

My proposal is to use the existing corpus of Martin's previous books as a basis for producing an algorithmically-generated version of <em>The Winds of Winter</em>. 

This has a few potential forms, depending on what results I have success in creating. Ideally, I'd like the <code>TWOWbot</code> to capture the tone of Martin's previous work (something Olde English sounding). If that's possible then <code>TWOWbot</code> will produce "quotes," likely assigned to point-of-view characters (utilizing my previous TF-IDF analysis of the books). Failing that, I'd like the bot to capture another part of Martin's sensability: his relentless plot twists (and willingness to murder beloved characters). In this case I'd like each tweet to summarize some sort of plot twist. This seems model seems to lend itself to using context-free grammars.

And we're off.

&1F44D;