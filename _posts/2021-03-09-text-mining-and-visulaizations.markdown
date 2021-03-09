---
layout: post
title:  "Text Mining, Visualization, and Comparison"
date:   2021-03-09 11:51:00 -0500
categories: 
---

Text mining and visualization tools can be great for finding patterns and trends across Latin inscriptions!...when they work. I ran into issues this week with getting around 23 of my cleaned inscriptions input into the text mining tool *Topic Modeling Tool*, but had more success uploading everything into *Voyant*. My goal this week was to do some text mining and comparative analysis of a small sample of Latin inscriptions from the african provinces and a poem by the satyrist Martial.

## The Inscriptions

The inscriptions I worked with this week all originated from CIL III in the provinces of Creta, Cyrenacia, and Alexandria. I uploaded a total of 22 cleaned inscriptions with notations on province of origin, particular find spots, and the character count of the inscriptions. It should be noted that the character counts do include the null spaces in the plain text, which unfortunately means that the counts are higher than is accurate. Nevertheless, the margin of error is minimal. One inscription which gave an initial character count of 36, when hand counted, produced an actual count of 26 characters.
Below is one example of the inscriptions used in this week's experiment.

> **Province of Origin:** ALEXANDREA 
>
> **Inscription Number:** 19
>
> **Find Spot:** Alexandreae rep. a. 1746.
>
>DOMINI NOSTRI INVICTISSIMI ET VENERABILES
>AC PERPETVI AVGVSTI THEODOSIVS ET 
>ARCADIVS TOTO ORBE VICTORES 
>MATERNO CYNEGIO OMNIVM VIRTVTVM VIRO ET AD 
>INSIGNEM LAVDEM GLORIAMQYE•PROGENITO• PER 
>OMNES • HONORVM. GRADVS • MERITORVM CON 
>TEMPLATIONE PR.OVECTO PRAEFECTO  
>PRAETORIO PER ORIENTEM STATVAM 
>CIVILI HABITV AD PETITVM PRIMORVM NOBILIVM 
>ALEXANDRINAE VRBIS IN EADEM SPLENDIDA  
>VRBE AD PERPETVITATIS FAMAM LOCO CELE 
>BERRIMO CONSTITVI coLLocAmoys IVSSERVNT 
>PER CLARISS/IMOS AL/EXANDRINAE CIVITATIS 	
>
>**Character Count:** 493

The special benefit of the above inscription (CIL III 2.1.19) is that it is the only one in the sample which includes a distinctly feminine title *materno*, mother. 

I ran this and 21 other inscriptions through Voyant with the below results:

![CIL III Voyant Text Graph](C:\Users\profg\CILImages\CIL_III_Voyant)

This graph demonstrates the frequency of familial phrases, such as "son" or "mother" in the sample corpus.

![CIL III 2.1.19 Voyant Text Graph](C:\Users\profg\CILImages\CIL_III_Voyant2.1.19BreakDown)

This graph focuses on inscription 2.1.19 to demonstrate the frequency and correlation of the word "mother" with phrases denoting glory, fame and honor.


## The Comparative Text

I chose to compare this particular inscripition set with a poem by the satyrist Martial known simply as Martial 10.63. The poem itself is a parody of a funerary epitaph for a noble woman, and thus serves as a good comparison.

>Marmora parva quidem, sed non cessura, viator,
>Mausoli saxis pyramidumque legis.
>Bis mea Romano spectata est vita Tarento,
>et nihil extremos perdidit ante rogos:
>quinque dedit pueros, totidem mihi Iuno puellas, 5
>clauserunt omnes lumina nostra manu¯s.
>Contigit et thalami mihi gloria rara fuitque
>una pudicitiae mentula nōta meae.
>
>Martial 10.63

Below is an english translation, in case you're interested in reading any Martial today. Beware the euphamisms!

>10.63  EPITAPH OH A NOBLE MATRON:
>
>Small though the tomb, traveller, on which you read these lines, it yields not in interest to the sepulchres of Mausolus or the Pyramids. I have lived long enough to be twice a spectator of the Secular Games; and my life lost nothing of happiness before my funeral pyre. Juno gave me five sons, and as many daughters; and their hands closed my dying eyes. Rare conjugal glory, too, was mine; my chaste love knew but one husband.

Obviously this is meant to be a humorus and raunchy poem, but it holds to the conventions of inscriptions fairly well. As evidenced by Voyant, it also holds correlations to the same themes od chastity, honor, and glory which we find in inscription 2.1.19. As an added bonus, it also references the pyramids of Egypt, and the above inscription was uncovered nearby the pyramids.

![Martial Voyant Text Graph](C:\Users\profg\CILImages\Martial_Voyant)

## The Conclusion

Ultimately, this experiment revealed some interesting comparisons of terminology. Had I gotten the proper text mining tool working, it is likely that my experiment would have yeilded clearer results. But even for a start which was, admitedly, biased (afterall I was aware that 2.1.19 clearly refered to a woman before I even started) I think that text mining like this could prove promising as I contiune with this project.

