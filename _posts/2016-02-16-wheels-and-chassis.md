---
layout: post
title: Hot Wheels
image: /img/2016-02-16-wheels-and-chassis.jpg
---

For the first couple weeks of Reinventing the Wheel I've worked on prototyping a set of four wheels and corresponding chassis. I fabricated my wheels from scratch, but used pre-fabbed components to build the chassis. 

I've made it a goal this semester to improve with CAD, so I plan on modeling all of projects for this class. My weapon of choice will primarily be Fusion 360, since it largely duplicates SolidWorks' approach to solids modeling and parametric design, but has also has the major advantage of being free. I'm also taking a SolidWorks (and ZBrush) workshop over at LaGuardia Studio, which so far has been helpful.

I did some research into hubcaps and rims for some inspiration, and decided on a general design, but I didn't get into specifics until I started modeling. I decided to put a sloping inward taper on one of the faces, which wound up being quite a challenge, but I got basically what I wanted with what I assume was the least efficient methodology possible. The hub fits a quarter-inch shaft, and on the back face there's an inset space for a bearing.

<figure>
<a href="https://lh3.googleusercontent.com/NDx6UcZdTb9fPKk9lBAbv7-jips1paZtkkNIJsXyd6HzaYpPuTGCN8Lr8HciGhgZED9Qm2ZRG0i9G8AP1GvCDAhwiW0SHV7uGVOBH3rBMv7HPEWSaPhSzEJvVc2MIKaT3PzAnsL43fHkeY3HWzm1b8qGL5GYkcwhUCvqmkCdbOq8lUldRfyw0-T4wKpiNPS8uz98J8pCkjDKaqxjyNFu7j1_-vRNcu4u1hfbWOGmaH57CbYX2tiAjr8vStEzeMhN9ozbOiIYbqZVrj9sj0_o9EChgIFrzo7YOPzCDaQ2T3SL_Wha9GFZyrqv-6OnyrMg_AT5X-t0kmIuZGIeMaRyXg0oBfparQQEgDiZql4X0s8YOHvAX8-2R04seBCv_pmMf-anoDXfWqD0tFX4uhykY77Zc-YxcTa-dtqT6BjX6i2DYZidaKWSIrj_uXQXfgAcTBG6V-PosDt4-XqKCnD2PkQHSzv2Dhe4s1_B5bsjYQQ-yfX8cALh1WSfdhopBTTXllqXR0sZmiQfy6p0Wnme8gm5vpOyyRUDCm1F2JbOdMBUZluVD9ur9iR3oMSwaCimsM1X=w534-h334-no" data-lightbox="CAD Model" data-title="My initial model. Notice the inward-sloping taper.">
	<img src="https://lh3.googleusercontent.com/NDx6UcZdTb9fPKk9lBAbv7-jips1paZtkkNIJsXyd6HzaYpPuTGCN8Lr8HciGhgZED9Qm2ZRG0i9G8AP1GvCDAhwiW0SHV7uGVOBH3rBMv7HPEWSaPhSzEJvVc2MIKaT3PzAnsL43fHkeY3HWzm1b8qGL5GYkcwhUCvqmkCdbOq8lUldRfyw0-T4wKpiNPS8uz98J8pCkjDKaqxjyNFu7j1_-vRNcu4u1hfbWOGmaH57CbYX2tiAjr8vStEzeMhN9ozbOiIYbqZVrj9sj0_o9EChgIFrzo7YOPzCDaQ2T3SL_Wha9GFZyrqv-6OnyrMg_AT5X-t0kmIuZGIeMaRyXg0oBfparQQEgDiZql4X0s8YOHvAX8-2R04seBCv_pmMf-anoDXfWqD0tFX4uhykY77Zc-YxcTa-dtqT6BjX6i2DYZidaKWSIrj_uXQXfgAcTBG6V-PosDt4-XqKCnD2PkQHSzv2Dhe4s1_B5bsjYQQ-yfX8cALh1WSfdhopBTTXllqXR0sZmiQfy6p0Wnme8gm5vpOyyRUDCm1F2JbOdMBUZluVD9ur9iR3oMSwaCimsM1X=w534-h334-no" alt="CAD Model" title="My initial model. Notice the inward-sloping taper.">
</a>
<figcaption>My initial model. Notice the inward-sloping taper.</figcaption>
</figure>

I manufactured the wheels using the Roland 4-axis CNC mill. The priority here was efficiency, so I simplified the cutting as much as possible. I wound up able to stick with larger tools, using a quarter-inch square end mill for roughing, and a quarter-inch ball nose mill for 99.9% of the finishing. Because the Roland CAM wizard is both limiting and unwieldy, I couldn't cut the inset for the bearing to finished depth while roughing, and the ball nose couldn't reach all of it, I wound up having to switch back to a square mill at the end for what came out to maybe 30 seconds of cutting. Tools changes on the Roland are pretty slow, so having to make an extra one was an obstacle, but since I would have had to change back to the square mill before cutting the next wheel anyway, it all worked out.

<figure>
<a href="https://lh3.googleusercontent.com/mDoGt7oKCtf8IYX9WqAN4kFbUMllaRr1ec7eCDvIUlaFWWq76nM_EsauPDQtmgrLGKNpM3PUr5-ORX5tN2nNlyk6QXSj3FfsTrknK7ws1LpCXf6fMrxMXQ_07J0_tDhaS4_KMstZpG3RW9cakg4b8EBoY1D_VAgwVwqBojoQ4O9S_BdsrQi2FBmOnMKQZ9xpOfl7qOwxvy7_bbcDbXqtNOSlZIFIY-Jv8PjGBYrh_tCJiSVPu38muqz3Ei7hzhO29ZLq4aaftirVswIehkrE_UA4942rlBFSLn3uS5uHm3wpb-voh72V9UVSz4VnFGg3yAtqoEGf3cPjtdpd_4sCfBwzgRtdl8xMZ7PO7MxrkMVDgJbkGfJaEjqTyAzPZQM3h6Q3lN_NGEL6nl5ge_FLilOiRbt1Gt6O_MSkiBHqcigtdUTHNf7QGDoq99Y6sgtvb_3UGz_tf1WuPJ6g3JROBCvAm_CWoT0rWiDn-LP0Lcy5CdMKmzKUm8EI_oNUQIMu2v9E8EIN5Z-nU73UWZeFm4HiNITSchfawN3OZvqrFLbixKITxaAKw-6jNjdBCaDwz47B=w2148-h1610-no" data-lightbox="Rough cut" data-title="Rough cutting a wheel.">
	<img src="https://lh3.googleusercontent.com/mDoGt7oKCtf8IYX9WqAN4kFbUMllaRr1ec7eCDvIUlaFWWq76nM_EsauPDQtmgrLGKNpM3PUr5-ORX5tN2nNlyk6QXSj3FfsTrknK7ws1LpCXf6fMrxMXQ_07J0_tDhaS4_KMstZpG3RW9cakg4b8EBoY1D_VAgwVwqBojoQ4O9S_BdsrQi2FBmOnMKQZ9xpOfl7qOwxvy7_bbcDbXqtNOSlZIFIY-Jv8PjGBYrh_tCJiSVPu38muqz3Ei7hzhO29ZLq4aaftirVswIehkrE_UA4942rlBFSLn3uS5uHm3wpb-voh72V9UVSz4VnFGg3yAtqoEGf3cPjtdpd_4sCfBwzgRtdl8xMZ7PO7MxrkMVDgJbkGfJaEjqTyAzPZQM3h6Q3lN_NGEL6nl5ge_FLilOiRbt1Gt6O_MSkiBHqcigtdUTHNf7QGDoq99Y6sgtvb_3UGz_tf1WuPJ6g3JROBCvAm_CWoT0rWiDn-LP0Lcy5CdMKmzKUm8EI_oNUQIMu2v9E8EIN5Z-nU73UWZeFm4HiNITSchfawN3OZvqrFLbixKITxaAKw-6jNjdBCaDwz47B=w2148-h1610-no" alt="Rough cut" title="Rough cutting a wheel.">
</a>
<figcaption>Rough cutting one of my wheels.</figcaption>
</figure>

I used birch plywood stock since that was all I had laying around, but I didn't decide on that before modeling. If I had I could potentially have factored the thickness of the laminate into my design, which would have given me some interesting surface patterns, but I didn't end up with much contrast this way. I initially used ten layer ply, but I decided to try one with some five layer material. Honestly, there wasn't much of a difference, although there may have been slightly more tear out with the five layer. I only encountered one significant void, and conveniently it was in an inauspicious area of the back face of the wheel.

<figure>
<a href="https://lh3.googleusercontent.com/aMfvCOwLaC4MUq8OyHVwKS8mvF8gRakSLvVUO1HvGOmVRVPfKA1yPcFbBsDyGNjuoZ-7YGvJEIiU=s1610-no" data-lightbox="After roughing" data-title="After rough cutting.">
	<img src="https://lh3.googleusercontent.com/aMfvCOwLaC4MUq8OyHVwKS8mvF8gRakSLvVUO1HvGOmVRVPfKA1yPcFbBsDyGNjuoZ-7YGvJEIiU=s1610-no" alt="After roughing" title="After rough cutting.">
</a>
<figcaption>After rough cutting</figcaption>
</figure>

<figure>
<a href="https://lh3.googleusercontent.com/wqDi-YiatSw99b3u1Icrto2RDmW1autVX8g1yqZVpUAvhss7sd3gk8SOWGAzrqY78eBwHm79lozobDhcflArmWkv9vvrjkBuC8_CEvJTCJlemybwuEGfKoTZlSsH9ZD2DX6lifd9VdjFeNNo_7re-n4IO5YoiKr1SbpI90EpruIRfDSVYdN2vyGFZ-baLmB0abQ3m4k6WwY29VLuO0VC9qrVtGFJGsFUM5lfVF1Cd3B0TXteIK4qGc6Ua0Eibe1F3lAiyqm9t4URhyhl_s3tYlOqqGcI8Dt86nv_6ayNETA-qE2hcueR-3npkrnvH7QeZuXqkGwz5_tYnmYdRg8JeoaLclNfHwFnchKOBjVPAAeSMvGolGGuiisMGI3ldo7pjP9H-9zdIX4U9Jyo82_rD0aDSlY1vDvzbQ8uevCCMsI77i8oSVGyccS5DKKUOGxnlEJN9jZQH6QzaebZGVuRGPw0_ncQvFzsYW4HpDGsfchoSJo9PxhkxecYRcTWaYcVeh19K1bhqWYOdfr9_ZE0Hz8n81Hsy24ePQpZb7cwDTnbn0eK5ekzHQZ8u5hmk-eJyCUT=w2148-h1610-no" data-lightbox="Finished" data-title="The finished job.">
	<img src="https://lh3.googleusercontent.com/wqDi-YiatSw99b3u1Icrto2RDmW1autVX8g1yqZVpUAvhss7sd3gk8SOWGAzrqY78eBwHm79lozobDhcflArmWkv9vvrjkBuC8_CEvJTCJlemybwuEGfKoTZlSsH9ZD2DX6lifd9VdjFeNNo_7re-n4IO5YoiKr1SbpI90EpruIRfDSVYdN2vyGFZ-baLmB0abQ3m4k6WwY29VLuO0VC9qrVtGFJGsFUM5lfVF1Cd3B0TXteIK4qGc6Ua0Eibe1F3lAiyqm9t4URhyhl_s3tYlOqqGcI8Dt86nv_6ayNETA-qE2hcueR-3npkrnvH7QeZuXqkGwz5_tYnmYdRg8JeoaLclNfHwFnchKOBjVPAAeSMvGolGGuiisMGI3ldo7pjP9H-9zdIX4U9Jyo82_rD0aDSlY1vDvzbQ8uevCCMsI77i8oSVGyccS5DKKUOGxnlEJN9jZQH6QzaebZGVuRGPw0_ncQvFzsYW4HpDGsfchoSJo9PxhkxecYRcTWaYcVeh19K1bhqWYOdfr9_ZE0Hz8n81Hsy24ePQpZb7cwDTnbn0eK5ekzHQZ8u5hmk-eJyCUT=w2148-h1610-no" alt="Finished" title="The finished job.">
</a>
<figcaption>The finished job.</figcaption>
</figure>

I took off the majority of the tab material with a handsaw, but entirely evening the surface of the wheel required a power tool. As another issue I wish I had designed for, I didn't have a proper mount for the lathe, so I had to improvise a bit. I used a bolt as a makeshift arbor, and then held that arbor in a Jacobs chuck, which I could fix to the headstock. It was only a taper mount though, so it was not an ideal set up, but fortunately I only needed to just touch the wheels with a gouge; any more and this likely wouldn't have held up. The rest was sandpaper. 

<figure>
<a href="https://lh3.googleusercontent.com/prRv-vSkiU0qk8eMqN9-nOiH1qTw6ldyrGxR4_KUV9JFVBQLw9hP_d43I7-_zLB6fSWljxtgQetPElrrz2jJaUhlQ6uKdIQnjEnP5nwAb06jkEO7k7TWfn7TD8JpxkQJvRPETe0uqyuXXrkFuJ-VfHflwkEOYqQWlwuNKwZLfY4yzPIng5B0fR11DIwboCgE6zPWDLbKKQNOAIuKwxYZnJ7qimW-o17sot7zLZ3hFV2skjjzApYjFFAgwifAKUTQQspJGDWc9jWzfwrcdaYr-3yNfPe5Vv0Rrte9bvuAkVk_BtO0RxZYD6sK0OZeNdpwn3GmN9Nukz2MSbjqa6tfLqpGRY1cnCQ2ujjdpnnG3N8A1hn0ThDPeSB5UjYrus6xHc_cCHqe0OJAgzhdqtlIgmf33KteZTH9bPAwyqqIpVATu4CMKJfmE2DxwG5RKCJrKUb-FrGmh19ObQaSPXnEaw37k4IUavP8GtnDto2WVF0ybOg-rUBzPDhaGxcnq57wBsntwzUzWrSHr_vBxboppGew0rdhFcBAkomRmqf3wcnJdbe34M5YcOgZ-FYDjw5TyTTc=s1610-no" data-lightbox="Jacobs chuck" data-title="My improvised mounting solution.">
	<img src="https://lh3.googleusercontent.com/prRv-vSkiU0qk8eMqN9-nOiH1qTw6ldyrGxR4_KUV9JFVBQLw9hP_d43I7-_zLB6fSWljxtgQetPElrrz2jJaUhlQ6uKdIQnjEnP5nwAb06jkEO7k7TWfn7TD8JpxkQJvRPETe0uqyuXXrkFuJ-VfHflwkEOYqQWlwuNKwZLfY4yzPIng5B0fR11DIwboCgE6zPWDLbKKQNOAIuKwxYZnJ7qimW-o17sot7zLZ3hFV2skjjzApYjFFAgwifAKUTQQspJGDWc9jWzfwrcdaYr-3yNfPe5Vv0Rrte9bvuAkVk_BtO0RxZYD6sK0OZeNdpwn3GmN9Nukz2MSbjqa6tfLqpGRY1cnCQ2ujjdpnnG3N8A1hn0ThDPeSB5UjYrus6xHc_cCHqe0OJAgzhdqtlIgmf33KteZTH9bPAwyqqIpVATu4CMKJfmE2DxwG5RKCJrKUb-FrGmh19ObQaSPXnEaw37k4IUavP8GtnDto2WVF0ybOg-rUBzPDhaGxcnq57wBsntwzUzWrSHr_vBxboppGew0rdhFcBAkomRmqf3wcnJdbe34M5YcOgZ-FYDjw5TyTTc=s1610-no" alt="Jacobs chuck" title="My improvised mounting solution.">
</a>
<figcaption>My improvised mounting solution.</figcaption>
</figure>

<figure>
<a href="https://lh3.googleusercontent.com/XCB-CXqFtB54UNxOcb2sjwvGWDSnQ2GeCQizkZH7hp5VUud7-IIZHSPndlqbkrKkqUMDfUPYT0Y5P3TvUstmR4CYPl44OP_fOkRAHZQ7yXgCQklSD84YwHiT1C-bXfiWANJjRA4UlGhi7dPOjb_tPD0qYaZ168EL9zESqOr-XP2_5X_YVlpPk177ANNvKb1SocUn9JK95F1Bo4hYY-pYDH9bRYmYB_PRu4enLhml_YE2s8nMDyJPnZkOuuM0umcpxTcnp5jCruno4cg4rqDFyZ6tXvqI79UiOrOmkjmcmjxR1uXIybKeUL2B9RV-IiUq_4-Srqd6ccAArvWL5-D9LfCMibqyG89aSEMmr3C19cgTc0a4usFOgMrxQU-1gSe9r_Z5Px4DMDuXR9w_CnLN9xkJgr_jTOwZvGvOVKud7RgikXQ6Raljtc3LjW-b_nQacsuztFLvz8sz3vV65P1GbfgX6WpDZrlZw65svGYoZuQTsR6JOsMICOGWx2sHqCqms53jFkBQzmudjKOafVdTFQQt4wegCXaifVQhZiAmHJT0W0CoyrVaBISCSGqaI6LPbSvL=s1610-no" data-lightbox="Four wheels" data-title="All four wheels complete.">
	<img src="https://lh3.googleusercontent.com/XCB-CXqFtB54UNxOcb2sjwvGWDSnQ2GeCQizkZH7hp5VUud7-IIZHSPndlqbkrKkqUMDfUPYT0Y5P3TvUstmR4CYPl44OP_fOkRAHZQ7yXgCQklSD84YwHiT1C-bXfiWANJjRA4UlGhi7dPOjb_tPD0qYaZ168EL9zESqOr-XP2_5X_YVlpPk177ANNvKb1SocUn9JK95F1Bo4hYY-pYDH9bRYmYB_PRu4enLhml_YE2s8nMDyJPnZkOuuM0umcpxTcnp5jCruno4cg4rqDFyZ6tXvqI79UiOrOmkjmcmjxR1uXIybKeUL2B9RV-IiUq_4-Srqd6ccAArvWL5-D9LfCMibqyG89aSEMmr3C19cgTc0a4usFOgMrxQU-1gSe9r_Z5Px4DMDuXR9w_CnLN9xkJgr_jTOwZvGvOVKud7RgikXQ6Raljtc3LjW-b_nQacsuztFLvz8sz3vV65P1GbfgX6WpDZrlZw65svGYoZuQTsR6JOsMICOGWx2sHqCqms53jFkBQzmudjKOafVdTFQQt4wegCXaifVQhZiAmHJT0W0CoyrVaBISCSGqaI6LPbSvL=s1610-no" alt="Four wheels" title="All four wheels complete.">
</a>
<figcaption>All four wheels complete.</figcaption>
</figure>

From there it was on to figuring out a chassis. Unfortunately that section was rushed, so I don't have any in-process photos. In a stroke of luck I found an aluminum hard drive sled on the junk shelf. Not only was it sturdy, it also had two round indentations on each side, perfectly aranged for an axle. I've ordered another hard drive tray; this might be a recurring thing. I drilled out the holes, and the space wound up being a perfect fit for the bushings I planned to use. The wheels fit very snugly on the axle, but I added a shaft collar on either side to make sure they stayed fixed. 

And the end verdict? It rolls!

<figure>
<a href="https://lh3.googleusercontent.com/GFV5926LREzZvy4VLxi9IQJRyNj8xN1UwmKh4c6vJuH81bS0mINmaVTy0litM_bdcFk9R3AzYUesLndLO28w_-aPok-lNba5A2Q4i0--03R-1adKypoTJhNVLW4_PrIVhzIWWSiGQOYQMvLzF4VAeao1o4QcUt7PfavmeWwcr2TX8Du29_l1qXfbKLaNRJqKVBk2R0m675iTnVyLBXUL3Zm6-FgzYN0KobIW16f2Dk5d011vtoOPnNVuJKmOUAF41WaIGSv3Hn0USkWk876OEKRhVV__V3azz584IRT-7KJRWFsvTxCHDWDiwdWP_hFJj3IulAh6JNwyeHcXE_s4Q5siagzEsgJ7WRdROXs0cY2PgXqzH538JHRERvKFif7uS8so72jW0lKuTU9c_Qz1JgcJPRVZkOlgp0DoVYNp5qFsMnuTqNib6A69J27jiTNdhf8ZzxEZmBp4IDMSqfvRGg1_9-gYEsorQ4JM-1WjqjbD91moTy-EZ6iA-ehGnoRvPT-umhclJR_wC0XSOQObFvSyX1_WkQmTA4RcT1ni5hKx-4GyJ4xo39poqZbDR0u4eJ0U=s1610-no" data-lightbox="Wheels on chassis" data-title="The finished assembly.">
	<img src="https://lh3.googleusercontent.com/GFV5926LREzZvy4VLxi9IQJRyNj8xN1UwmKh4c6vJuH81bS0mINmaVTy0litM_bdcFk9R3AzYUesLndLO28w_-aPok-lNba5A2Q4i0--03R-1adKypoTJhNVLW4_PrIVhzIWWSiGQOYQMvLzF4VAeao1o4QcUt7PfavmeWwcr2TX8Du29_l1qXfbKLaNRJqKVBk2R0m675iTnVyLBXUL3Zm6-FgzYN0KobIW16f2Dk5d011vtoOPnNVuJKmOUAF41WaIGSv3Hn0USkWk876OEKRhVV__V3azz584IRT-7KJRWFsvTxCHDWDiwdWP_hFJj3IulAh6JNwyeHcXE_s4Q5siagzEsgJ7WRdROXs0cY2PgXqzH538JHRERvKFif7uS8so72jW0lKuTU9c_Qz1JgcJPRVZkOlgp0DoVYNp5qFsMnuTqNib6A69J27jiTNdhf8ZzxEZmBp4IDMSqfvRGg1_9-gYEsorQ4JM-1WjqjbD91moTy-EZ6iA-ehGnoRvPT-umhclJR_wC0XSOQObFvSyX1_WkQmTA4RcT1ni5hKx-4GyJ4xo39poqZbDR0u4eJ0U=s1610-no" alt="Wheels on chassis" title="The finished assembly.">
</a>
<figcaption>The finished assembly.</figcaption>
</figure>