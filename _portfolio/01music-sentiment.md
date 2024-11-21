---
title: "Music Sentiment Analysis"
excerpt: "Predicting Music Emotion from Social Media Commentary<br/><img src='/files/wordcloud.svg'>"
collection: portfolio
---

Assessing the affective quality of a piece of music is a difficult task, generally relying on expensive surveys to collect user annotations on how they feel about a given song. Determining these emotional ratings is a task of interest to the music information retrieval community, as such information enables the development of better music recommender systems towards the goal enabling automatic music therapy solutions.As such, prior works including [AMG1608](https://ieeexplore.ieee.org/document/7178058), [PmEmo](https://dl.acm.org/doi/10.1145/3206025.3206037), and [DEAM](https://cvml.unige.ch/databases/DEAM/) provide musical samples manually annotated for valence (happiness) and arousal (energy) characteristics. In their 2018 paper, [Deezer](https://arxiv.org/pdf/1809.07276.pdf) sought to automate this process, using NLP analysis of song lyrics and analysis of acoustic features to predict music [valence and arousal](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2784275/). We look to expand on this work by using social media conversations to predict music affect.

In 2021, we presented preliminary findings at [NCUR](https://www.cur.org/what/events/students/ncur/). Our initial approach at this learning task relied on parsing these comments using existing word affect and valence/arousal dictionaries like the work presented by [Warriner et. al.](https://link.springer.com/article/10.3758/s13428-012-0314-x) and generating summary statistics based on the aggregate total of valence/arousal words in a comment to create a feature space. This yielded modest performance towards the task of music emotion recognition, and demonstrated the feasibility of estimating dimensional music emotion targets without relying on acoustic features.

![NCUR 2021 Poster](/images/beery_poster.png)


This work has been conducted as part of [Soundbendor Lab](https://soundbendor.org/) @ OSU-Cascades, advised by [Dr.
Patrick Donnelly](https://engineering.oregonstate.edu/people/patrick-donnelly)
