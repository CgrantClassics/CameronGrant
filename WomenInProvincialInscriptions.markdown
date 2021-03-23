---
layout: page
title: Women in Roman Provincial Inscriptions
permalink: /WomenInRomanPI/
---

## The Project and the Goal

A project with the ultimate goal of digitizing the Corpus Inscriptionum Latinarum (CIL) volumes II and III so that they can be filtered for the study of women living in the provinces of ancient Rome. All volumes of the CIL digitized here are out of copyright, and have become outdated with new additions to the CIL corpus.

The Corpus Inscriptionum Latinarum is a vast collection of inscriptions collected from across the Roman world in a variety of ancient languages. The inscriptions are recorded as they are preserved, with some restoration by modern epigraphists. The text of the CIL is fully in Latin, with no translations of the inscriptions available in the printed additions.

Digitizing CIL corpus of Latin Inscriptions from the provinces of Spain, Egypt, and Asia in the hopes of creating a database for women in the Roman Mediterranean world.

Final corpus digitized using Fine Reader OCR, with a smattering of Google OCR.

Volume Abbreviations | Volume Number | Locations
-------------------- | ------------- | ---------
CIL II | Volume 2 | Inscriptions from Roman Spain
CIL III | Volume 3, Part 1 | Inscriptions from Roman Egypt and Asia



*Disclaimer*: This project is being done as I dip my toes into the realm of computational methods for Humanities research. I claim neither mastery nor accuracy at this point in time, this is an artifact of the learning process. 


## The Material: Considerations and Issues

Epigraphy and inscriptions are unlike literary sources, in that they were written (or rather, paid for) by individuals whose voices may not survive in any other state. At the same time, they should not be taken at face value. Inscriptions were expensive and dedicated for several reasons including:
1. Repaying a vow to the gods
2. Eulogizing a desceased loved one
3. Memorializing a great accomplishment or event, and
4. Begging aid from the gods


For these reasons, inscriptions tend to idealize the people and events for which they are dedicated and thus must be treated carefully. What these texts can reveal, however, are overarching patterns of and purposes for dedication. These patterns could be revealing when studied in conjunction with patterns of women's appearances in these inscriptions in the roles of *Dedicator* and *Dedicant*.


It should also be noted that the inscriptions collected in the CIL volumes consist of both epigraphic inscriptions (created professionally and paid for by the dedicator) and *graffito* which are inscriptions and drawing created by an average citizen that were not necessarily created for an express purpose.


## The Material: Products of Digitization


#### The Printed Artifact

I began this project using the scanned texts of CIL II and CIL III from [HathiTrust](https://catalog.hathitrust.org/Record/100029672). These records are now obsolete as newer additions have been released, and are thus out of copy right. In terms of digitization, the corpus poses a few unique issues. 
1. The inscriptions are printed as closely as possible to their state of preservation. This means that some inscriptions are missing sections, have sections which were reconstructed by scholars, or have breaks in them which do not translate to OCR. 
2. The printed pages themselves are split into columns and sections which cause confusion for most OCR programs. I finally settled on using [ABBYY Fine Reader](https://pdf.abbyy.com/finereader-pdf/trial/) which is more adept at running OCR on tables and columns.
Below are two images of the actual printed pages of the CIL volumes. You can see why the formatting may prove difficult for text recognition softwares that read from left to right!

![CIL II](/CameronGrant/Assets/CIL_II_OgPrintPage.png)
Fig 1: CIL II 

![CIL III](/CameronGrant/Assets/CIL_III_OgPrintPage.png)
Fig 2: CIL III


#### The Provinces in Question

The inscriptions from CIL II were recovered from Roman Spain-- *Hispania*-- (light blue circle). The inscriptions from CIL III were uncovered in Roman Egypt and Asia-- *Aegyptus et Asiae*-- (dark green). Thus far I have only worked with the inscriptions from the African provinces captured in the region as shown on the map below.

![Provincial Map](/CameronGrant/Assets/RegionMap.png)
The detailed map above depicts the provinces of the Roman Empire during the reign of Trajan who died in 117 CE. This was the Empire's greatest extent.

[Original Map](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/Roman_provinces_trajan.svg/1732px-Roman_provinces_trajan.svg.png)

#### Digitizing: OCR and Plain Text

The OCR plain text that is produced both by Google and by Fine Reader have their issues, but the clean products also have their own unique markers which need to be addressed before moving forward.

Character/Symbol | Meaning in Clean Text
---------------- | ---------------------
`/` | Break in the physical inscription
`///` etc. | Dashes inscribed within the inscription
`#, *, +` | A drawing in the inscription


In a backwards fashion, I started my digitization process with CIL III. For the sake of consistency, I will do so again now.

The final products of my digitization process can be found on my [GitHub](https://github.com/CgrantClassics/CameronGrant/tree/main/Inscriptions).

For an idea of what a full digitization of the CIL volumes looks like, check out the [Arachne Project](https://arachne.uni-koeln.de/drupal/?q=en/node/291)! I am working with the same volumes as the Arachne team, though at a much smaller, and novice, scale. Their goal is to fully digitize and make accessible these volumes, my own is to 1) learn the process, 2) produce inscriptions that are searchable for the purposes of gender theory studies.


#### **CIL III: Egypt and Asia**

I ran my first sections from this volume through Google's OCR by uploading PDF files to Google Drive and opening as a Google Doc. I had to splice each page in half with [Sejda](https://www.sejda.com/split-pdf-down-the-middle) to account for the columns. The process was long and repetitive, but it got the job done... sort of.

![CIL III Plain Text, Un-Cleaned](/CameronGrant/Assets/CIL_III_DirtyPlainTxt.png)

As you can see from the above image-- which covers the same inscriptions from Figure 2-- the OCR scan from Google copied each line twice along with invisible formating and peices of dirt-- all those strange symbols at the top? The orignial scan was probably dirty or grainy!. The quality of the lines had no rhyme or reason and the process of cleaning by hand was arduous, but doable with a copy of the scan at hand.

![CIL III Plain Text, Cleaned](/CameronGrant/Assets/CIL_III_CleanPlainTxt.png)

I cleaned each section and indicated the larger provincial region, and then the specific province name. I then ensured that each inscription was condensed into a single line. As you can see, there is a great deal of information included in each inscription. I logged the archival data along with the inscription in the following manner for each inscription, a "tab" space between each category:

Inscription # | Find Spot (if applicable) | Body of Inscription 
------------- | ------------------------- | ------------------- 

Some inscriptions did not include a known find spot. In these cases I inserted a double tab to leave that column blank. This process means that the inscriptions can now be easily copied into a program like Excel... and it produces a neat little table as well!

![CIL III Table Example](/CameronGrant/Assets/CIL_III_TableExample.png)


The end product of digitization and cleaning produces something like this:

> VII. CYRENAE (Gretna).  
> (cf. C. I. Gr. 5129-5183).  
> 8	 • Cyrenis ad aedem Apollinis. 	IVLIAE - AVGVSTAE CYRENENSES P-OCTAVIO-PROCOS 
> 9	 Cyrenis. 	 pONT • MAX • TRIB NI M FACTA 
> 10	 litteris magnis in epistylio, Cyrenis. 	 PORTICVS • CAESAREI • Restituit IVS• M • F • PACILAEVS L  


#### **CIL II: Spain**

The scans of this volume were run through Fine Reader, and the results of the scans were vastly improved.

![CIL II Plain Text, Un-Cleaned](/CameronGrant/Assets/CIL_II_DirtyPlainTxt_FineReader.png)

There are no double lines, and the scan clearly picked up on the columns without smooshing them together (smooshing is, of course, a highly technical term).

I went through the process of hand cleaning the text again. This text is more condusive to automating the cleaning process through the use of [Regular Expressions](https://regex101.com/), but by this point I was in the zone of cleaning by hand. The results are clearly similar in appearance to CIL III.

![CIL II Plain Text, Cleaned](/CameronGrant/Assets/CIL_II_CleanPlainTxt_FineReader.png)

> I. OSSONOBA (Faro).
> 1 		IMP • CAES • P • LI CINIO-VALERI ANO-P-F-AVG-PONT MAX- P • P • TR • POT• III COS • RES • P • OSSON EX • DECRETO • ORD DEVOTa•NVMINI M AI ES T A T I EIVS  	
> 2		 M • CORNELIVS • ERIDANVS • C-IVNIVS • RECEPTVS OBHONOREM • IIIIIVIR • D • S • P • D •  	
> 3	 	d • m • s c • A n n I v s R O M V L V S ANNORVM XXVIII H-S-E-S-T-T-L 	


Obviously this is a far cry from the sort of information which I can use to find women in these inscriptions; however, it's the sort of data which I can run through analysis tools that *would* produce useful results for the sort of research I am working on.