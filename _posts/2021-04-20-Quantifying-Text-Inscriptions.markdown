---
layout: post
title:  "Quantifying Text Based Inscriptions"
date:   2021-04-20 11:49:18 -0500
categories: 
---

Everything is quantifiable, or at least that's what Lemercier and Zalc tell us. Any data set, any corpus, can be quantified and analyzed in some way. But can you quantify text?

Sure you can! There are a great many ways one can go about it. In the case of my current project- wherein I am serching for women in inscriptions- this may seem a tad unhelpful. Since my corpus is not yet at a point where I can build a data table out of my whole corpus quantification will look fairly... off topic.

In the future I could see it being very helpful! Once my corpus is clean and I can properly search through it I could build a quantifiable data set for say... every instance of the word *filiae*, or "daughter", across all Latin inscriptions from Spain, Egypt, and Asia. Gee... wouldn't that be swell? One day it will be.

But for now, I am experimenting with quantification through a program known as R-Studio in a direction that is somewhat less relevant for the purposes of actually learning how to use the tool.

**This week's quantification goal:** How do the lengths of inscriptions vary across Roman provinces in Egypt and Northern Africa?


## The Experiments


I worked exclusively with inscriptions from CIL III for this foray into R-Studio. The process itself was... complicated to say the least. Working with the coding language "R" was entirely new territory for me, and the guide I was using was somewhat outdated for the version of the program I was running, but thanks to a great deal of adivce, patience, and the figurative bashing of my head against a wall... I managed to load up my .csv files (that is, comma seperated value workbooks I created in Excel) to R-Studio and run its graphing programs. I will add a disclaimer here that my particular data set (province / region names and character counts) was not condusive to the creation of fancy bar graphs or area graphs. I stuck to the tried and true scatter plot.

# The Data Points, Provinces, and Charts

I created my visualized quantifications for a series of inscriptions from two distinct provinces in Northern Africa

* Creta and Cyrenaica: 11 inscriptions
* Alexandria: 20 inscriptions

Obviously, there's a big disparity in sample size here which is typically frowned upon in statistical analysis. The disparity, however is a bit less important in this case given that it is the unavoidable nature of the corpus, and I am also not looking to compare either region quite yet.

I first loaded my data sets into R-Studio to produce the following tables:

**Creta and Cyrenaica**

![Creta Table](CameronGrant/Assets/RStudio_DataFrame_CIL_III_Creta.png)

**Alexandria**

![Alexandria Table](CameronGrant/Assets/RStudio_DataFrame_CIL_III_Alexandria.png)

These tables are known as data frames, and they're what R-Studio's "ggplot" package will turn into pretty charts and graphs. I've listed relevant info such as the inscription's call number; its province, city, or region of origin; the full body of the inscription; and an accurate character count (spaces are not counted as characters).

I elected to quantify this data to see what I could observe about inscription lengths across regions. Since several of the inscriptions are from the same area, they are counted as one entity on the x-axis of my chart.

* X-Axis: City or Region of origin
* Y-Axis: Character count

These graphs should show me a general pattern of inscription length which could theoretically be used to determine cost of inscriptions.
