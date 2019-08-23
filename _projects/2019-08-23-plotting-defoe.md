---
layout: project
title: "Plotting Defoe's Adventure Novels"
author: inachen
tags: [projects]
img: defoe-map.png
description: >
display-order: 1
---

[Project Link] (https://redadvance.github.io/defoe-map/)

---
## I. Inspiration
My research project was an emotion map of Daniel Defoe’s adventure novels. The novels used were *Robinson Crusoe (1719), Captain Singleton (1720)*, and *Colonel Jack (1722).* The map was meant to show the emotions associated with locations mentioned (not necessarily visited) in these books . The inspiration for this project was an emotion map created by Christian Nold. His maps represented the emotions, opinions and dialogue of the local population. The map was drawn from a pile of drawings made by the people in the city to portray their perception of the place they live in. I was fascinated by how he managed to combine this static and hyper-accurate medium with something as abstract and ambiguous as human emotions. I wanted to create something similar to Christian Nold’s map: a world map of the 18th-century drawn from the passages of Defoe’s novels.
## II. Research Questions and Motivations
I chose this project because I was curious about Britain’s relationship with other countries at that time, primarily Spain and France. I wanted to see if these novels accurately portray British sentiments towards outsiders by comparing fiction with nonfiction (travel literature). I was aware that Britain held a great deal of  anti-French sentiment during the 18th-century and I wanted to see if Defoe’s novels portrayed a similar feeling towards the French. My original research question was centered around what emotions are associated with which location and why, but that question seems far too broad, but I ultimately narrowed my question down how Defoe describes these locations and how his descriptions evoke a negative, positive or neutral emotion. At the end of the 10-week internship, I had created a map, while not up to the level of Nold’s artistry, does include a positive, negative or neutral rating for the locations mentioned in the three Defoe novels I finished analyzing.
I soon realized my earlier methods were too time consuming so I sought for a more machine-oriented way to streamline the process. My new method involved NER tagging the text (taken from Gutenberg) then locating the passages with those location tags and running those passages through two sentiment analysis tools before providing my own score of that passage. The two sentiment analysis tools used were Vader and Stanford sentiment analysis tool. Vader seems to provide a more positive rating while Stanford mostly gives out negative ratings to the passages. I then used ArcGIS to create a map for Defoe’s novels, which has different layers for each novel followed by separate layers for Vader, Stanford and my score of that novel. This method focused on locations mentioned in the text rather than the actual location the characters were in.
---
<img src="{{site.baseurl}}/img/crusoe-map.png">
---
<img src="{{site.baseurl}}/img/defoe-map.png">
---
As I continued working on this project, I added a secondary project using AntConc. I found out that if I collocate (finding the most frequent words around a certain word) a location word then I could get peripheral words that provide a general idea of the author’s description of that location. For example, in Robinson Crusoe, when I did a collocation search for the word  ‘Africa,’ the most frequent words to appear were: vulgarly, enterprises, productions, leopards, sailors, desert, tigers, shipwrecked, perished, lions, skins, misfortunes. These words painted Africa as a wild and dangerous place that was also very profitable. Another example was the location word ‘Sallee’ which produced the results: Turkish, Turks, rovers, moors, war, emperor, devoured, prisoners. This provided a very negative illustration a place controlled by the Turks who were barbarians that took prisoners. This is supported 18th-century British sentiments towards the Turks.
I also created a website to store and organize all my data, my progress reports, and the methods and tools I used for this project. The site provided an overview of what my project was about, my inspiration for it and guides for downloading and using the NLP tools. I also posted updates on my progress and had a place to upload my location tagged files. The website was made with google sites classics.
## IV. Results and Reflections
From the Defoe’s map, I noticed that England and London produced neutral sentiments, which made sense since those locations were where the characters started out. Spain, France, Africa, and the Caribbean Islands had incredibly negative sentiments. This correlated with Britain’s rivalry with Spain and Africa and their prejudice towards Africa as a wild and uncivilized place. The Caribbeans also had pirates that pillaged merchant ships during the  18th-century. I also found out that Defoe saw places like London and Lisbon as mercantile locations or locations primarily used for business transactions.
There were a couple of problems with my method. First, it was tedious work. I had to find all the passages with the location tag one at a time and run them through each of them through a sentiment analysis tool. Luckily Alice came up with a method to cut down on the amount of work using a text editor and google sheets to separate each passage with a location tag into single lines. The second problem was that a passage would contain multiple locations. For this, I would look at whether this passage was relevant in that it has some emotion attached to it rather than just listing a bunch of locations visited. Then if that passage was deemed relevant, I would simply analyze the same passage multiple times for each location in it. Another problems was that sentiment analysis tools were mainly used for social media tweets and not large bodies of text from 18th-century. Vader tended to provide a more positive rating and rarely gave a neutral rating while Stanford sentiment analysis tool almost always gave a negative rating. More than once, I defaulted to my own judgement of the text which can be biased since I have read some of the novels rather than analyzing the passage as an isolated text apart from the novel.
If I were to continue with this project, I would want a more streamlined and less tedious and time-consuming way to analyze a large corpus rather than simple four or five books. I also would want to more in depth emotions in my map like anger or sadness. I wanted to figure out a way to attain more nuanced emotions from the text beyond just rating the passages as negative, positive or neutral. Furthermore, I wanted a way to link the data points to a page with the passage it came from so that the reader can interpret the text themselves.
## V. Works Cited
Cjhutto. “Cjhutto/VaderSentiment.” *GitHub*, 22 Apr. 2018, github.com/cjhutto/vaderSentiment.
Saldaña, Zoë Wilkinson. “Sentiment Analysis for Exploratory Data Analysis.” *Programming Historian*, 15 Jan. 2018, programminghistorian.org/en/lessons/sentiment-analysis#
Exploring-text-with-sentiment-analysis.
Heuser, Ryan., et al. “The Emotions of London.” *Stanford University*, Oct. 2016.
Nold, Christian. “Stockport Emotion Map.” 2007, http://stockport.emotionmap.net/map.htm.
## VI. Works Consulted
Bridges, Roy. “Exploration and Travel Outside Europe (1720-1914).” The Cambridge Companion to Travel Writing, edited by Peter Hulme and Tim Youngs, Cambridge University Press, Cambridge, 2002, pp. 53–69. Cambridge Companions to Literature.
Sherman, William H. “Stirrings and Searchings (1500-1720).” The Cambridge Companion to Travel Writing, edited by Peter Hulme and Tim Youngs, Cambridge University Press, Cambridge, 2002, pp. 17–36. Cambridge Companions to Literature
Wall, Cynthia. "Travel Literature and the Early Novel." *The Oxford Handbook of the Eighteenth-Century Novel*, J. A. Downie, Oxford UP, 2016, pp. 121-136. Oxford Handbooks (Oxford Handbooks).
## VII. Credit
I would like credit Alice, my supervisor, for providing me with a more streamlined method of extracting passages with the location tag from the text. I also would like to credit Scott Enderle for helping me figure out the steps I needed to take in order to analyze the emotions of the text.

The project site can be found [here](https://redadvance.github.io/defoemap/).
