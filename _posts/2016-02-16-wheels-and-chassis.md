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
<a href="https://lh3.googleusercontent.com/fmql7_t9Dk3mjTEX3JdS2S3me9PGF3FzgN5mJTbPHgIzUmMQal4wQvq_SFaksEf7Y1NQ8drNn1Ad6SEKMIvs0-Znf-oHsDCj2H5jQejbKO4I3jZcWOgkTWaAGjwNHO7PxSeMflAvtVeAX2Dg1Fq-bRZptdAoUBy1PwbAsfC3q560qd0VkTIbT3bPZjQ4eoZlJRaFbqBxLS7raXL8-juwOZhkq2x5UwIqSsUI-cTvEVK-aDhzq6UUrFW3KVD-j1K6VAr7o7cpi7L-KULnHM1-TxYahcfeW0X0TO8kwwKKfDDy3PUNKpblEl0ZzTvZ2J7btIxQVLLthAFuAf3vZcFgsjyWGZJmUVCvNe5iRG-mK6ut6NkgjbF47NWdA5kwMahwL_j6a7xLvREg6uGcWXpLmqlm8TPrXMfg3QmXY3Jotp1vGxjj63TKuabtPDMEOFqt_sGdKWy_YWh0Os6Lbqlwl-GCwyoMJN68ayZEwajx7_aKCA8DajJMtQ8FOeuo23U8gaPxsCz6zJNBMFGdKYzl31UxWKSgutgqtMPzmlCGCkVYvPJ7jWf-VOgGaGrLkKuNzFsy=w2148-h1610-no" data-lightbox="Finished" data-title="The finished job.">
	<img src="https://lh3.googleusercontent.com/fmql7_t9Dk3mjTEX3JdS2S3me9PGF3FzgN5mJTbPHgIzUmMQal4wQvq_SFaksEf7Y1NQ8drNn1Ad6SEKMIvs0-Znf-oHsDCj2H5jQejbKO4I3jZcWOgkTWaAGjwNHO7PxSeMflAvtVeAX2Dg1Fq-bRZptdAoUBy1PwbAsfC3q560qd0VkTIbT3bPZjQ4eoZlJRaFbqBxLS7raXL8-juwOZhkq2x5UwIqSsUI-cTvEVK-aDhzq6UUrFW3KVD-j1K6VAr7o7cpi7L-KULnHM1-TxYahcfeW0X0TO8kwwKKfDDy3PUNKpblEl0ZzTvZ2J7btIxQVLLthAFuAf3vZcFgsjyWGZJmUVCvNe5iRG-mK6ut6NkgjbF47NWdA5kwMahwL_j6a7xLvREg6uGcWXpLmqlm8TPrXMfg3QmXY3Jotp1vGxjj63TKuabtPDMEOFqt_sGdKWy_YWh0Os6Lbqlwl-GCwyoMJN68ayZEwajx7_aKCA8DajJMtQ8FOeuo23U8gaPxsCz6zJNBMFGdKYzl31UxWKSgutgqtMPzmlCGCkVYvPJ7jWf-VOgGaGrLkKuNzFsy=w2148-h1610-no" alt="Finished" title="The finished job.">
</a>
<figcaption>The finished job.</figcaption>
</figure>

I took off the majority of the tab material with a handsaw, but entirely evening the surface of the wheel required a power tool. As another issue I wish I had designed for, I didn't have a proper mount for the lathe, so I had to improvise a bit. I used a bolt as a makeshift arbor, and then held that arbor in a Jacobs chuck, which I could fix to the headstock. It was only a taper mount though, so it was not an ideal set up, but fortunately I only needed to just touch the wheels with a gouge; any more and this likely wouldn't have held up. The rest was sandpaper. 

<figure>
<a href="https://lh3.googleusercontent.com/Y5x7IeSH-OsJ7prsgkC3GcgeVDsZrgtv6Kv4jN4khHihv-9v-WzmixRT00ecrQ5LgOgFsWFztZhZM6ZfegNIroKQGX8aUr1coTB1Y8dLb_6RzStZO-Cn5iJRJJwvxP55JzCHosWm_9mCKMSWTjCjGyIqXbYY7HNm-I4aohXtdCbC77KpUaDVCKGp_eF0LcW3lkyY9SzQ8F30M2Xc3bAxE1FZP3HaHTCa1Sow6mvBDRTN02gynXYZ7UJae9Z61jlQtDwtihzF0jT4ybML1SUCDCD29mYquWJ6nIaRCiCBdf3qsZLwFi_YaP46_xzdPkHeEejatzt2nthO6G17xZskhdVIM1Ev1Y_UryY1dstsydxFRmSn576pnsXUZadP2muqHA6sknkLdTTPOYOiWu3ZPzcI6y0u2wlZBHGUvIB3AmIaICnJXbJFZ6YUp7n94azR-TfMLJAHQjsUZAs6IZ2S7_qYb3VIg8J8BkjRNt3n0_vEBpNKYu6Lq8aX93-ByO929TlD0RLr9dysp8yWlr_slm_FpoFRefvJu8sPNWunCK5ReTm659HXRxkfDLeEbt4Efh2b=s1610-no" data-lightbox="Jacobs chuck" data-title="My improvised mounting solution.">
	<img src="https://lh3.googleusercontent.com/Y5x7IeSH-OsJ7prsgkC3GcgeVDsZrgtv6Kv4jN4khHihv-9v-WzmixRT00ecrQ5LgOgFsWFztZhZM6ZfegNIroKQGX8aUr1coTB1Y8dLb_6RzStZO-Cn5iJRJJwvxP55JzCHosWm_9mCKMSWTjCjGyIqXbYY7HNm-I4aohXtdCbC77KpUaDVCKGp_eF0LcW3lkyY9SzQ8F30M2Xc3bAxE1FZP3HaHTCa1Sow6mvBDRTN02gynXYZ7UJae9Z61jlQtDwtihzF0jT4ybML1SUCDCD29mYquWJ6nIaRCiCBdf3qsZLwFi_YaP46_xzdPkHeEejatzt2nthO6G17xZskhdVIM1Ev1Y_UryY1dstsydxFRmSn576pnsXUZadP2muqHA6sknkLdTTPOYOiWu3ZPzcI6y0u2wlZBHGUvIB3AmIaICnJXbJFZ6YUp7n94azR-TfMLJAHQjsUZAs6IZ2S7_qYb3VIg8J8BkjRNt3n0_vEBpNKYu6Lq8aX93-ByO929TlD0RLr9dysp8yWlr_slm_FpoFRefvJu8sPNWunCK5ReTm659HXRxkfDLeEbt4Efh2b=s1610-no" alt="Jacobs chuck" title="My improvised mounting solution.">
</a>
<figcaption>My improvised mounting solution.</figcaption>
</figure>

<figure>
<a href="https://lh3.googleusercontent.com/Lji9IiW313TG4fcwxBI3BMXJBAZQqMIga-d5fZwpZl-LvvUm0XJt4yddxjINpnHtqFS1UwMFZiGZPpMHDR8Eh7EwS0Hqaul69d-lCfBTMxpj1JBSzTtUw4HoD18ViHlrgfDlJ7iSP5FgKRWMtPg40OEBM-y6zR0LGvIz5BMMEn7uX3s-boRDUcSSgaLCFUhCeR4De0a9iAUt8f1SJdtuQVVRvqPhu87ziud3LakBeOpESm04_HAVTQRqf0-dMnJ1dK44h2GpY3we0q4t851k8rSlGyRsS6yJT4-0fR4Y6Xg_eyo9iOJzPmGC2WUER3EHsOPF_azgNrU9HbUS_k20_fy00Yt_XQs8Bouj-3fKSJQTzhS41A_o8GHYxDyo-nmj21732Wbf1E-rPbk_pWiLOQwE5IIR9beyhStIe1ojf1RQ4kKVqHuze12yQTvZo0o7Hq56jz1WPdoEssJHCKrtl_S6U8zBBus_6I9sykX_GrMYUf3J-fH_cW0q_wNG9tIzpPuN41G9Tp6mDtlrwQs-wbV9briRpWKb7Y22pO2ax0beLXOhZFSTTNGEDVpoQJAskV5_=s1610-no" data-lightbox="Four wheels" data-title="All four wheels complete.">
	<img src="https://lh3.googleusercontent.com/Lji9IiW313TG4fcwxBI3BMXJBAZQqMIga-d5fZwpZl-LvvUm0XJt4yddxjINpnHtqFS1UwMFZiGZPpMHDR8Eh7EwS0Hqaul69d-lCfBTMxpj1JBSzTtUw4HoD18ViHlrgfDlJ7iSP5FgKRWMtPg40OEBM-y6zR0LGvIz5BMMEn7uX3s-boRDUcSSgaLCFUhCeR4De0a9iAUt8f1SJdtuQVVRvqPhu87ziud3LakBeOpESm04_HAVTQRqf0-dMnJ1dK44h2GpY3we0q4t851k8rSlGyRsS6yJT4-0fR4Y6Xg_eyo9iOJzPmGC2WUER3EHsOPF_azgNrU9HbUS_k20_fy00Yt_XQs8Bouj-3fKSJQTzhS41A_o8GHYxDyo-nmj21732Wbf1E-rPbk_pWiLOQwE5IIR9beyhStIe1ojf1RQ4kKVqHuze12yQTvZo0o7Hq56jz1WPdoEssJHCKrtl_S6U8zBBus_6I9sykX_GrMYUf3J-fH_cW0q_wNG9tIzpPuN41G9Tp6mDtlrwQs-wbV9briRpWKb7Y22pO2ax0beLXOhZFSTTNGEDVpoQJAskV5_=s1610-no" alt="Four wheels" title="All four wheels complete.">
</a>
<figcaption>All four wheels complete.</figcaption>
</figure>

From there it was on to figuring out a chassis. Unfortunately that section was rushed, so I don't have any in-process photos. In a stroke of luck I found an aluminum hard drive sled on the junk shelf. Not only was it sturdy, it also had two round indentations on each side, perfectly aranged for an axle. I've ordered another hard drive tray; this might be a recurring thing. I drilled out the holes, and the space wound up being a perfect fit for the bushings I planned to use. The wheels fit very snugly on the axle, but I added a shaft collar on either side to make sure they stayed fixed. 

And the end verdict? It rolls!

<figure>
<a href="https://lh3.googleusercontent.com/qpq1wkO-uzCuKT5EClyIoNNPLwVfKwMjoUm3ZwZGZHtvTJNfhEMgZCJy308FIEKanie2PKlAP7hPIGttAU3FB83sXSE8q8Gaom-S5T4MeBpCagyj1Yl0mdbEF5LtbqfjqVe5ARMX4HyPs4kAOS-QMNI_W_yYPyzJR39pPxTCbsKfz5Gh2-DvN9S2xBZ_YqEZS5TGdM8QJkFbgy2erTfs_LQZiXcu9bA89r2EArZBWhOctaBrdlAZqFLZ0SX-W_Xpmf2muim7b0DCaOWU3huLfNufjmu5qnkJQvcU7kgtv11ZjA-Y7O79IWGD5R6twCcZg-0oW_deCTsN7EWABGuzVjmSGKBLGJYOSCl_GXIaCZSbEjU6fKYXmQElpqKyYElzSO0En52HnFQGe91-4SPrGPWukFCUFlASQdoiLNJMOdp0ogGY3Qool5zhTeCpBkRHT5KU6X8FM8oRaTmTrhd06wahpRqS84mi9HX2pYlP2YzxznZHxjNIQQMSbxD5TAKEVchSkOSkaixQ0e7mOk3fyF_NdZgR_x_5_rasaGU-uHjCxexnZijIpPVOO3dwXDifycVb=s1610-no" data-lightbox="Wheels on chassis" data-title="The finished assembly.">
	<img src="https://lh3.googleusercontent.com/qpq1wkO-uzCuKT5EClyIoNNPLwVfKwMjoUm3ZwZGZHtvTJNfhEMgZCJy308FIEKanie2PKlAP7hPIGttAU3FB83sXSE8q8Gaom-S5T4MeBpCagyj1Yl0mdbEF5LtbqfjqVe5ARMX4HyPs4kAOS-QMNI_W_yYPyzJR39pPxTCbsKfz5Gh2-DvN9S2xBZ_YqEZS5TGdM8QJkFbgy2erTfs_LQZiXcu9bA89r2EArZBWhOctaBrdlAZqFLZ0SX-W_Xpmf2muim7b0DCaOWU3huLfNufjmu5qnkJQvcU7kgtv11ZjA-Y7O79IWGD5R6twCcZg-0oW_deCTsN7EWABGuzVjmSGKBLGJYOSCl_GXIaCZSbEjU6fKYXmQElpqKyYElzSO0En52HnFQGe91-4SPrGPWukFCUFlASQdoiLNJMOdp0ogGY3Qool5zhTeCpBkRHT5KU6X8FM8oRaTmTrhd06wahpRqS84mi9HX2pYlP2YzxznZHxjNIQQMSbxD5TAKEVchSkOSkaixQ0e7mOk3fyF_NdZgR_x_5_rasaGU-uHjCxexnZijIpPVOO3dwXDifycVb=s1610-no" alt="Wheels on chassis" title="The finished assembly.">
</a>
<figcaption>The finished assembly.</figcaption>
</figure>