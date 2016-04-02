---
layout: post
title: Expanding Ring
image: /img/2016-04-02-ring.jpg
---

The assignment this week was a wheel that did "more than just roll and spin," so I set out to build ring-shaped mechanism that would expand and contract while remaining circular. I based my design on some of Chuck Hoberman's [patent drawings](http://www.google.com/patents/US5024031) for expandable structures, which, coincidentally, were responsible for some of my favorite childhood toys.

Despite looking quite complex, the ring design is actually quite straightforward; the design I used only involved a single shape, repeated and mirrored.

<figure>
<a href="https://lh3.googleusercontent.com/LE1pgnqoUHHXamDVYm3VOJRBJsEDc1e1fG1gnhN6jM66NrtNWunePHgPR-oEzinalgeUySYJBaaT1YxYfEevSpWvYHkGOiGP3EnwUxzbqhkdn15yipSHnCUTN4XgC1rbyc7vzOJuXemQEmDfueDnQbvBlXYo95WYC-VJ5vNDhUaZ7Nk8qX9qwrqic3sGvqhC3rgqBIuzGNaDFnvwceU0LG87foCDRzTtgEbGn0JpVLABzCeaqjMX48iZV1ux9nKEciKrEOhg80RZATgu-dDY-pBlGczLwuDB-Y7qAnuK0ijG6K8zOPztV5Xh1S4CN3_IyDbfldPyi5DBwYN8fX0fu83qy5fTeN3mqnJ_GFWGm0oCe0GVbFWI-rHgB7JEvZVyEx18ATjS1OthiaHcUdIK6slrvJ82otYcxTOe4lqowvscuCbi33nT-GNiZ_9L4UvCYvhWNXggIO6W8KWdi2P9DFzRgX56q4BHzoVnveB0MKru0HBK3lkv8qh8EWGaOS1gvCaroaTqfKtNk1Tr5acm_4ANA4LSG6OKzVf68UCWONhmW3EJksOYVXPwRp-hgmSa1Kui=w2576-h1610-no" data-lightbox="Basic shape" data-title="This was the only sketch I needed for my CAD. I produced all the components from the same design.">
	<img src="https://lh3.googleusercontent.com/LE1pgnqoUHHXamDVYm3VOJRBJsEDc1e1fG1gnhN6jM66NrtNWunePHgPR-oEzinalgeUySYJBaaT1YxYfEevSpWvYHkGOiGP3EnwUxzbqhkdn15yipSHnCUTN4XgC1rbyc7vzOJuXemQEmDfueDnQbvBlXYo95WYC-VJ5vNDhUaZ7Nk8qX9qwrqic3sGvqhC3rgqBIuzGNaDFnvwceU0LG87foCDRzTtgEbGn0JpVLABzCeaqjMX48iZV1ux9nKEciKrEOhg80RZATgu-dDY-pBlGczLwuDB-Y7qAnuK0ijG6K8zOPztV5Xh1S4CN3_IyDbfldPyi5DBwYN8fX0fu83qy5fTeN3mqnJ_GFWGm0oCe0GVbFWI-rHgB7JEvZVyEx18ATjS1OthiaHcUdIK6slrvJ82otYcxTOe4lqowvscuCbi33nT-GNiZ_9L4UvCYvhWNXggIO6W8KWdi2P9DFzRgX56q4BHzoVnveB0MKru0HBK3lkv8qh8EWGaOS1gvCaroaTqfKtNk1Tr5acm_4ANA4LSG6OKzVf68UCWONhmW3EJksOYVXPwRp-hgmSa1Kui=w2576-h1610-no" alt="Basic shape" title="This was the only sketch I needed for my CAD. I produced all the components from the same design.">
</a>
<figcaption>This was the only sketch I needed for my CAD. I produced all the components from the same design.</figcaption>
</figure>

I also took this as an opportunity to explore joint simulation in Fusion 360, which wound up being pretty interesting. This model had a lot of joints – 32 of them, to be specific, all of them revolute – so the simulation became understandably processor-intensive. I was able to resolve that by applying a limited range of motion to each joint, but I still having problems; for reasons that I couldn't understand at the time, whenever I went to attach the final joints, my simulation would fail. I wound up with an almost-but-not-quite complete circle, and while all the other joints were working, the mechanism behaves quite differently without those final connections, as you can see below.

<iframe src="https://player.vimeo.com/video/161264977" width="676" height="535" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

I posted my problem on Autodesk's forums and got some very helpful responses. We weren't able to nail down a single specific cause, but there are a couple potential culprits: First, the circular pattern likely confused Fusion. In order to run the simulation, a component of the mechanism had to be "grounded," and this mechanism would likely be easier to articulate if I could ground it to a center point, which unfortunately isn't an option. Second though, my geometry may have been causing some problems. The patent drawings I followed didn't have any specific numbers included, so there's definitely a possibility that I messed up a dimension that prevented the assembly from aligning correctly.

Despite being unable to simulate it, the model still seemed eminently buildable – being able to introduce some slop to joints helps – so I went for it. I laser cut the components from a sheet of presentation board, an exceptionally dense cardboard that was tricky to find good settings for. Still, except for the char marks it worked well, and I took care of those with a coat of spray fixative. The joints are connected using folding brass fasteners. Lo and behold, it works!

<figure>
<a href="https://lh3.googleusercontent.com/I3B7A7BbEZt8vKuUEauK6OZf7gdQqPcMEJ6YGz6JKGU0eBB-x-X6E3YDg0j3xthqBdB2lmoJoOOGzSGGJ896h5z7EUQsI58FVmrr_svISBqirlqvDJr2BmuzIdBJwowxpGdPJoqA0Ib022ZgG9utu57FnKJhukXOv8Pt426pGlkPrP6onWtfbA93uAqK6mnqW4ccYtrCWFH5UoxwvGT7RLRgz99Wg_msUFdasbwMGBAJHW2GwFRtthjeJj4Uk6nMmHUD73diXifj7a54oPPkUxk4A6n5hiUXSb_QlEgxJ97eqDcmfwrhyjpxYxrGQI2cAM39AK-QGRCoD8lQOSaR9RHfmFDF8wB0peeapVPg3GEjI2ma9W9VOU21X4WNKhUXIjM4lB8CrA8hQlJs1ia4IVI1Oj3dq_3dVeaEISZGobQABzmb1Rpt5XmqFd9LAR7cJ51HfeOyS5qvBg-FS4Vtz2p9EAu4tNd6gttaCPioZzgPmMEluAglCYaHSvrXyYiaUq5K76OMmmxBF5J6J--p5tucLj8hgkMocOw17uUp7nuuYK1hGwlpujS6ukNcGNuXJZ0r=w2148-h1610-no" data-lightbox="Closed ring" data-title="Laser cut and assembled. In the closed position.">
	<img src="https://lh3.googleusercontent.com/I3B7A7BbEZt8vKuUEauK6OZf7gdQqPcMEJ6YGz6JKGU0eBB-x-X6E3YDg0j3xthqBdB2lmoJoOOGzSGGJ896h5z7EUQsI58FVmrr_svISBqirlqvDJr2BmuzIdBJwowxpGdPJoqA0Ib022ZgG9utu57FnKJhukXOv8Pt426pGlkPrP6onWtfbA93uAqK6mnqW4ccYtrCWFH5UoxwvGT7RLRgz99Wg_msUFdasbwMGBAJHW2GwFRtthjeJj4Uk6nMmHUD73diXifj7a54oPPkUxk4A6n5hiUXSb_QlEgxJ97eqDcmfwrhyjpxYxrGQI2cAM39AK-QGRCoD8lQOSaR9RHfmFDF8wB0peeapVPg3GEjI2ma9W9VOU21X4WNKhUXIjM4lB8CrA8hQlJs1ia4IVI1Oj3dq_3dVeaEISZGobQABzmb1Rpt5XmqFd9LAR7cJ51HfeOyS5qvBg-FS4Vtz2p9EAu4tNd6gttaCPioZzgPmMEluAglCYaHSvrXyYiaUq5K76OMmmxBF5J6J--p5tucLj8hgkMocOw17uUp7nuuYK1hGwlpujS6ukNcGNuXJZ0r=w2148-h1610-no" alt="Closed ring" title="Laser cut and assembled. In the closed position.">
</a>
<figcaption>Laser cut and assembled. In the closed position.</figcaption>
</figure>

Kind of.

The ring expands, but in order to do so, the entire assembly has to flex (actually, it flexes at the joints, which have plenty of play. I'm not sure what it would do if the joints were tight. Probably break, the way Fusion did.) The result more than fits my purposes, but I'm not sure at this point whether this is a part of the original design, or just a breakdown because of my attempt to copy it. Further research will be required, but in the meantime it's very satisfying to play with.

<figure>
<a href="https://lh3.googleusercontent.com/XFdp7GlmSHyAAqc_sgQOUfocfgHxODJEkVsr3g3b85SAnz2kboYeEC_xg3JBz_GZyhLeR-WizqdqxW-8FAy3hpVgALXbc2AYUgTrBgNGsKpjdtbA11zvNWnE21hYJqHvzEVN44FGi6kBfVTI_TppO9XIaQgr3yjbDvfJbXMxNQDwMcSSsMY4rgUyrOPfMXo9uMJbUpdYthkFC6mLOdjpa6qUd5SMw_5XbziXjo7Mji0SKxe1Q5bjBG7aqlqfRE9tH_FoyRessQiS9GlfO2Y8Hia5tst2j3iRRRTqQrK744WMzmn6MBBA3zYqH5SdTBiEdJs5gpUC5Y89Yppa5cNdTkCWNjlh0QmKeaVivrTcpirO-6gFIbiCHVzYgvdyEVpIXU_qyHcO8_XPzrm-T9YNm83U892gly0IsQHm7U77_WqeRo8-wI8ArRbabZUorJGpxLaJhBMOOYXt7I27Rr8Io57XgqX9g0iFObzzolooy0n02AramnAF6r8KvGMtHLvuP5vt9UXt7lws6yyC7sBJq9Lzgz15eA4kvV-4et1UVzN4WPZfUmUZOsjEKV3Igj7FZCTL=w2148-h1610-no" data-lightbox="Open ring" data-title="Fully expanded, and very much contorted.">
	<img src="https://lh3.googleusercontent.com/XFdp7GlmSHyAAqc_sgQOUfocfgHxODJEkVsr3g3b85SAnz2kboYeEC_xg3JBz_GZyhLeR-WizqdqxW-8FAy3hpVgALXbc2AYUgTrBgNGsKpjdtbA11zvNWnE21hYJqHvzEVN44FGi6kBfVTI_TppO9XIaQgr3yjbDvfJbXMxNQDwMcSSsMY4rgUyrOPfMXo9uMJbUpdYthkFC6mLOdjpa6qUd5SMw_5XbziXjo7Mji0SKxe1Q5bjBG7aqlqfRE9tH_FoyRessQiS9GlfO2Y8Hia5tst2j3iRRRTqQrK744WMzmn6MBBA3zYqH5SdTBiEdJs5gpUC5Y89Yppa5cNdTkCWNjlh0QmKeaVivrTcpirO-6gFIbiCHVzYgvdyEVpIXU_qyHcO8_XPzrm-T9YNm83U892gly0IsQHm7U77_WqeRo8-wI8ArRbabZUorJGpxLaJhBMOOYXt7I27Rr8Io57XgqX9g0iFObzzolooy0n02AramnAF6r8KvGMtHLvuP5vt9UXt7lws6yyC7sBJq9Lzgz15eA4kvV-4et1UVzN4WPZfUmUZOsjEKV3Igj7FZCTL=w2148-h1610-no" alt="Open ring" title="Fully expanded, and very much contorted.">
</a>
<figcaption>Fully expanded, and very much contorted.</figcaption>
</figure>

<iframe src="https://player.vimeo.com/video/161262254" width="676" height="380" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>