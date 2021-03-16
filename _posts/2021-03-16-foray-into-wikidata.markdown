---
layout: post
title:  "A Foray into WikiData"
date:   2021-03-16 4:06:18 -0500
categories: 
---

This week I dipped my toe into the wide world of Wikipedia. This was especially nerve-wracking considering I have always been warned that Wikipedia is the wild wild west of online encylopedias, and no place for an innocent young academic like myself. Oh well! Here we go!


## Wiki What Now?

WikiData is basically the source of your typical Wiki page, and where the bulk of my experimentation took place this week. The long and short of it is... I delved into the data enteries of my favorite Roman woman, Livia Drusilla, and played around with her entry. Honestly, I did have some qualms about her entry. For example, she is listed as having lived during the "High Roman Empire"... I strongly disagree with this. The High Empire is where we find the Third-Century Crisis. The Julio-Claudians (of which Livia was a matriarch) had nothing to do with it.

![WikiData Item page for Livia](/CameronGrant/Assets/Livia_WikidataPage.png)
Look! It's me, CGrant2021! Does this count as my first scholarly publication?


So! What to do? In the WikiData item for Livia Drusilla, first Empress of Rome, I found the entry for "time period" and added the designation of "principate"... Mwahaha! Okay so I may be being a bit dramatic, but it is interesting to see how these changes are made.

![WikiData Item "time period" for Livia](/CameronGrant/Assets/Livia_WikidataContribution.png)

This means that Livia now appears in query searches for an instances of humans from the *principate*, the time period from Augustus' ascendency in 27 CE all the way through to the *dominate* of 284 CE. This tag is far more accurate, since Livia is the first Empress of the period of the *principate*.


We can actually see that this worked by using WikiData's query service...

![WikiData query for "principate" and "female"](/CameronGrant/Assets/Principate_Female_Query.png)
Using Wiki's query service to search for instances of "female" within the time period of "principate" returns only one result: Livia!


Speaking of the query service, I also took some time this week getting to learn how to use it. I spent my time looking for instances which coincide with my research interests: women, the Roman Empire, and (for the sake of coheasion with this project) the provinces.


I began with a basic query for instances (that is items in the WikiData-verse) within the time period "Roman Empire" and with the designation of sex or gender "female".

![WikiData query for "Roman Empire" and "female"](/CameronGrant/Assets/RomanEmpire_Female_Query.png)

As you can see at the upper right, I have limited my search to 100 items, but there are definitely many more that could be found. At one point I went up to 300 items and I expect that I could go higher. Strangely, Livia was not counted amongst these women.

![WikiData query for "Roman Empire" and "female"](/CameronGrant/Assets/InkedRomanEmpire_Female_Query_LI.jpg)


I also added the filter for a place of birth in the province of Gaul as well as Hispania

![WikiData query for "Roman Empire", "female", "Gaul"](/CameronGrant/Assets/Locusta_Query.png)
![WikiData query for "Roman Empire", "female", "Hispania"](/CameronGrant/Assets/Melania_Query.png)

Clearly narrower searches return far fewer results. In the WikiDate-verse there are only two women who are tagged as having been born in these provinces during the period of the Empire: Locusta in Gaul (Nero's court poisoner and trainer of poisoners extraordinare!) and Melania the Elder in Hispania.


## Final Thoughts

Ultimately I think that the WikiData-verse and its query service could be extremely useful when searching for large datasets of particular categories and for their overlap with other large categories. Obviously, as evidenced by Livia's *exclusion* from the list of women in the Roman Empire, the tool is as perfect as its human editors. But then, isn't that the point? The more work we can put into making accurate tags and categories, the more accurate the results will be. I could see myself delving further into the WikiData-verse to help refine and fine-tune given the time and the confidence.