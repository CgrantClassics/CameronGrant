# CameronGrant
# *Current Project:* Women in Latin Provincial Inscriptions
Digitizing CIL corpus of Latin Inscriptions from the provinces of Spain, Egypt, and Asia in the hopes of eventually creating a database for women in the Roman Mediterranean world.

Final corpus will be digitized using Fine Reader, potentially with some Google OCR.

Cleaned and Finalized OCR available under "Clean OCR" folder.

A project with the ultimate goal of digitizing the Corpus Inscriptionum Latinarum (CIL) volumes II and III so that they can be filtered for the study of women living in the provinces of ancient Rome. All volumes of the CIL digitized here are out of copyright, and have become outdated with new additions to the CIL corpus.

Abbreviations | Volume and Location
------------- | -------
CIL II | Volume 2, Inscriptions from Roman Spain
CIL III | Volume 3, Inscriptions from Roman Egypt and Asia

**Corpus Segment Hierarchy**

Province/Region --> Individual Inscription

# Navigation

Most files on this repository are associated with running the website that brought you here! If you are looking for the corpus, look no further than the file named **Inscriptions**!

File Name | Description of Contents
--------- | -----------------------
Inscriptions | Home of cleaned and useable inscriptions in plain text format

# Dictonary

This section is used to record the syntax and phrases as well as any regular expressions or coding I use in the process of cleaning up my text. It is intended as a reference for myself in my work.

Syntax | Meaning
------ | -------
@@!@@ | Start raw material text
!!@!! | New region
`(?>I\.)`| Find Roman Numeral I followed by "." (Replace I with V,X,C as needed)
{| Replaces open parentheses
} | Replaces close parentheses
`([A-Z])\.\n(?=\n)` | Finds Capital Roman Numerals followed by "." and line break
`$1.` | Use to replace line breaks after Roman Numeral and preserves "."
`\d [A-Z BAR a-z]` | Find number followed by a space and either capital or lowercase letter (Finds Inscription archive number)
`\n$1` | Breaks above into lines based on inscription number

# **Progress**
2021-01-27: Uploaded plain text files from Hathi trust. Files are too large to view in raw format. Plan is to break up plain text into smaller files based on indexes and sections from original volumes

2021-01-29: Hathi plain text files missing hundred of pages. I ran the PDF through Adobe Acrobat's OCR scanner (Start - 12:05 pm; End - 3:30 pm). Will copy into plain text and proceed to break text into units for cleaning and research.

2021-02-01: Converted PDF in Acrobat to plain text file. Cleaning up plain text and breaking into units. CIL III converted to plain text, new file appears to be full plain text version of Hathi scans. On a fun note, the Chrome translate extension tried to translate the raw text from Latin to English, so the file is definitely readable! CIL II having issues... "untagged file" cannot be exported as a plain text file. Auto-tagging file through Adobe Acrobat and will attempt to export to plain text once file tagged (Start: 5:14 pm, End: 10:12 pm). Tagging potentially successful and I now have a plain text file exported, though it looks incomplete. Plan is to break PDF into smaller chunks and try again.

2021-02-02: Broke CIL II into 10 files (100 pages ea.); Ran OCR on smaller file, auto-tagged document, exported to plain text file... success! Plan is to convert rest of files and recombine plain text into 1 document in order to seperate based on region rather than random page numeration. CIL II files 1 - 4 completed (Start: 9:45 am, End: 1:11 pm). Cleaning up CIL III to remove library information and split file into multiple files based on regions as laid out in original publication (main unit of division). Sub-Regions in provinces typically deliniated by Roman Numerals. Find numerals, replace with `\n\n`

2021-02-03: Converted CIL II files 5 - 7 (Start: 8:15 am, End: 11:06 am)

2021-02-05: Converted CIL II files 8 - ? (Start: 8:28 am, End: 9:47 am). Files 9 - 10 are index material. Since this material is not relevant to the inscriptions, I will not be converting the files at this time.

2021-02-08: Regexr clean-up work

2021-02-09: Running CIL volumes through Google OCR... looks better but formatting is still difficult. Possibly to do with formatting on printed page, will need to look into solutions. Taking PARS PRIMA: CRETA ET CYRENAICA (2 pages/ 10 Latin inscriptions) from Google's OCR of first 20 pages of CIL III Aegyptus to clean by hand and run through OpenRefine. Ctrl F + H for `\n` and deleted all. Need to seperate into 1 inscription per line.

2021-02-10: Found a tool which corrects formatting issue called [Sedja](https://www.sejda.com/split-pdf-down-the-middle) which literally splits each page down the middle. Will split CIL II and III. This doubles page count. Will need to split each volume into 20 page sections in order to upload to Google for OCR work. (CIL II Start: 7:49 am; End: 11:20 am) (CIL III [parts 1 - 2] Start: 1:00 pm; End: 5:42 pm)

2021-02-16: Converting more CIL III PDFs to plaintext finished [parts 3 - 4 ] (Start: 8:25 am; End: 9:35 am). Cleaning up some of CIL III (Regions: Creta et Cyrenacia; Aegyptus et Aethiopia) to run through visualization tools. Replaced all capital "J" and "U" with "I" and "V" respectively as J/U do not exist in Latin alphabet. Worked in Tableu for some [visualization experiments](https://public.tableau.com/views/CILIIIParsPrimaSecvnda/Sheet14?:language=en&:display_count=y&:origin=viz_share_link). The plain text is not yet at a point where I think this type of visualization is useful, but the tool is definitely something to come back to once my data is cleaner.

2021-03-02: Having issues installing Jekyll through GitHub in order to create site for project. OneDrive does not play well with the command line prompts. Moved GitHub to local disk, and attempted to run my site locally `bundle exec jekyll serve --watch`, but this returned the prompt `Could not locate Gemfile or .bundle/ directory`. Update: I wasn't in the right folder. The local site is processing now. Editing and customizing my site. How exciting! And we're [live](https://cgrantclassics.github.io/CameronGrant/)!

2021-03-08: Working on text mining experiments. Ran into issue with Topic Model Tool. Reads `OutOfBoundException`. Potentially an issue with file size? Each file is 1 inscription, so very small. Will work on increasing file size by adding more files to folder and will try again later.

2021-03-09: Continuing work on text mining experiments. Potential issue identified. Designating files as `CIL_III_1.1.1` seems to have caused files not to save as .txt. Changing to `CIL_III_1_1_1` seems to have corrected file extention issue. All 22 files corrected to .txt extension. Still receiving same error. Could not get Topic Modeling Tool to work. Did experiments in Voyant instead.

2021-03-16: WikiData experimentation. Made a [blog post](https://cgrantclassics.github.io/CameronGrant/2021/03/16/foray-into-wikidata.html) for this week's experiments.

2021-03-18: Cleaning CIL III inscriptions (through CIL III 2.6.33). Created clean text and raw text files to upload to site for "middle product" documentation.

2021-03-23: Experimenting with [FineReader](https://pdf.abbyy.com/finereader-pdf/trial/) to see if it helps with the messy OCR... Update: OCR is *gorgeous*. It even allows me to set the scan language to Latin!! Unfortunately the free trial only allows me to scan 100 pages. Cleaning on CIL III done for this week (30 inscriptions, hand-cleaned), going to work on a chunk of CIL II. For sharing this week, I'm thinking I will enrich my source with a link to the arachne project, maps for the regions where the inscriptions were recovered, middle products (jpgs: PDF text, google OCR plaintext), and a link to the Hathi file. RegExr Cleaning CIL II Pars Prima: Ctrl F `Original from\nUNIVERSITY OF MINNESOTA`, Replace `\n`. Uploading inscriptions to personal site. This week's episode is live on my main [project page](https://cgrantclassics.github.io/CameronGrant/WomenInRomanPI/)!

2021-04-09: Doing some catch-up work on this project! Transferring relevant files from private to public facing repos.

**Work Log**
Date | Start Time | End Time | Total Time | Work Done
---------- | ---------- | -------- | ---------- | ----------------------------
2021-01-27 | 10:00 am | 10:30 am | :30 | Upload repo; Clean up README
2021-01-29 | 11:00 am | 12:10 pm | 1:10 | Sorting plain text; OCR scan PDF files
2021-02-01 | 10:14 am | 12:00 pm | 1:46 | Converting plain text; Clean up work
2021-02-02 | 8:30 am | 9:34 am | 1:04 | Break down CIL II; Convert plain text
2021-02-02 | 5:14 pm | 7:05 pm | 2:09 | Clean-up work CIL III
2021-02-03 | 8:15 am | 9:00 am | 1:15 | Converting CIL II; Clean-up work CIL III
2021-02-03 | 11: 00 am | 12:14 pm | 1:14 | Clean up work CIL III AEGYPTUS ET ASIAE
2021-02-09 | 4:29 pm | 7:02 pm | 3:27 | Hand cleaning; Open Refine experimenting
2021-02-11 | 8:00 am | 8:54 am | :54 | Transferring Google OCR to Sublime
2021-02-16 | 8:32 am | 9:35 am | 1:03 | Clean up work CIL III
2021-02-16 | 11:10 am | 11:59 am | :49 | Clean up work CIL III
2021-02-16 | 3:40 pm | 5:22 pm | 2:42 | Visualization work from cleaned CIL III
2021-03-01 | 4:30 pm | 4:52 pm | :22 | Building website for eventual display of results
2021-03-02 | 9:20 am | 12:05 pm | 2:45 | Building site
2021-03-02 | 3:10 pm | 3:34 pm | :24 | Building site
2021-03-08 | 3:00 pm | 5:44 pm | 2:44 | Text Mining Experiments
2021-03-09 | 8:52 am | 9:55 am | 1:03 | Text Mining Experiments
2021-03-09 | 11:00 am | 12:30 pm | 1:30 | Text Mining in Voyant
2021-03-16 | 3:03 pm | 4:56 pm | 1:53 | WikiData
2021-03-18 | 9:40 am | 10:29 am | :49 | Cleaning CIL III Inscriptions
2021-03-23 | 8:56 am | 9:30 am | :34 | Cleaning Inscriptions
2021-03-23 | 10:28 am | 11:03 am | :35 | Cleaning Inscriptions CIL II
2021-03-23 | 11:31 am | 11:50 am | :19 | Cleaning CIL II
2021-03-23 | 5:00 pm | 6:28 pm | 1:28 | Upoloading to Site
2021-03-23 | 7:06 pm | 7:54 pm | :58 | Uploading to Site
2021-04-09 | 9:40 am | 11:01 am | 1:21 | Transferring Corpus to personal repos. Updating Website Home page
2021-04-10 | 9:20 am | 10:41 am | 1:21 | Catch-up work - RStudio
2021-04-13 | 9:10 am | 9:37 am | :27 | RStudio
