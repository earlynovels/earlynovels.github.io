---
layout: project
title: "Epigraphs and Shakespeare in the 18th Century"
author: kirarasato
tags: [projects]
img: shakespeare-crop.jpg
description: >
---

This year, I centred my personal project on Shakespeare, my primary academic interest. Having recently completed a thesis on the legendary playwright, I had to ask this question: why were there so many Shakespearean epigraphs present in the eighteenth century? What is the significance of Shakespeare in this period? And is there a link between the function of the epigraph and the text itself.

For this, we should first go back to what an epigraph is, and why it is important to the eighteenth century. Epigraphs are, in essence, the first thing a reader encounters between the title of the book, and the main body of the novel-- sort of an "amuse bouche" of what is to come next. Something that is important to note here is that the epigraph is supposed to set the tone for reading, and what is to come ahead, and oftentimes, a famous quote from an Ancient Greek philosopher may be chosen to give the novel at hand more credence. In this, it can be argued that sometimes the epigraph is merely to be taken at face-value, in how it contributes to the overall construction of the novel. After all, if something is written in ancient Greek, it is unlikely that the majority of the growing population of readers in the eighteenth century would be able to read it.

What is also important to note is that, not only is the novel on the rise, but Shakespeare himself is gaining fast popularity amongst his eighteenth-century audience. Increasingly, Shakespeare was embedded in the literary canon, which gives rise to the question of whether the novel fed into the rise of Shakespeare, or vice versa.

From here, I used the END metadata to create .csv files to run through OpenRefine, a software designed to tabulate and parse through data fields. Using this tool, I was able to extract the epigraph information in the 591 fields of each record. Here, I started noticing that much of the data needed cleaning, and that data itself was not only subjective, but fallible.

After correcting the spelling mistakes, and double checking blank fields, I was able to find some interesting results. As it turns out, although Shakespeare was quoted the most, 40% of the time he was quoted, he was not attributed as the source of the quote-- a statistic that is almost equal to the 42% probability that Shakespeare was attributed as "Shakespeare". It was also not uncommon to find that the quote was just attributed to "Shakes." or "Shakespear." So what does this mean in terms of the authority of Shakespeare in the eighteenth century?

Even so, most of the records that did not attribute Shakespeare did reference the play that the quote was taken from, which engages with the idea that Shakespeare is commonplace knowledge at this time. But out of the 42 individual records, 13 records possessed neither attributions to Shakespeare or his plays. In these cases, then, I concluded that the text of the epigraph itself had to be significant in some way to the novel itself. Playing with a plain text version of "The recess" and mapping it against its epigraph from Shakespeare's As You Like It using Voyant Tools, I was able to find one specific portion of the text that contained all the words relating to the terms used in the epigraph-- a sort of primordial was of topic modelling, but an interesting result all the same.

What I can conclude from this is that epigraphs are not merely ornaments, but deliberate-- and something I wasn't really about to find the answer to was who was choosing the epigraphs in each novel in the first place.
