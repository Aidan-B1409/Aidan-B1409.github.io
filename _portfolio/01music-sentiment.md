---
title: "Music Sentiment Analysis"
excerpt: "Predicting Music Emotion from Social Media Commentary<br/><img src='/images/wordcloud.png'>"
collection: portfolio
---

Assessing the affective quality of a piece of music is a difficult task, generally relying on expensive surveys to collect user annotations on how they feel about a given song. Determining these emotional ratings is a task of interest to the music information retrieval community, as such information enables the development of better music recommender systems towards the goal enabling automatic music therapy solutions.As such, prior works including [AMG1608](https://ieeexplore.ieee.org/document/7178058), [PmEmo](https://dl.acm.org/doi/10.1145/3206025.3206037), and [DEAM](https://cvml.unige.ch/databases/DEAM/) provide musical samples manually annotated for valence (happiness) and arousal (energy) characteristics. In their 2018 paper, [Deezer](https://arxiv.org/pdf/1809.07276.pdf) sought to automate this process, using NLP analysis of song lyrics and analysis of acoustic features to predict music [valence and arousal](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2784275/). We look to expand on this work by using social media conversations to predict music affect.

In 2021, we presented preliminary findings at [NCUR](https://www.cur.org/what/events/students/ncur/). Our initial approach at this learning task relied on parsing these comments using existing word affect and valence/arousal dictionaries like the work presented by [Warriner et. al.](https://link.springer.com/article/10.3758/s13428-012-0314-x) and generating summary statistics based on the aggregate total of valence/arousal words in a comment to create a feature space. This yielded modest performance towards the task of music emotion recognition, and demonstrated the feasibility of estimating dimensional music emotion targets without relying on acoustic features.

![NCUR 2021 Poster](/images/beery_poster.png)

Improving upon this statistical approach, we use [BERT](https://arxiv.org/abs/1810.04805), a pre-trained language model,
to extract semantic information from our social media discourse. We train our model on a dataset of over 11.8 million
comments across Reddit, YouTube, and Twitter, each of which relates to one of 19,627 songs. We achieve state-of-the-art
performance on music valence/arousal prediction without relying on often-copyrighted acoustic data. You can find more
information on our experiments and results in our paper [here](https://aidanbeery.com/files/sact_2022.pdf)

![EECS 2022 Poster](/images/wine_poster_2022.png)

This work was supervised by [Dr. 
Patrick Donnelly](https://engineering.oregonstate.edu/people/patrick-donnelly) at [Soundbendor Lab](https://soundbendor.org/), Oregon State University.
