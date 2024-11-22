---
title: "Smart Compost Bin"
excerpt: "Developing a low-cost, 3D printed device for automatically measuring food waste using state-of-the-art computer vision models<br/><img src='/images/bin_thumbnail.jpg'>"
collection: portfolio
---

Food waste continues to strain the global food supply even as millions struggle with food insecurity. A lack of effective food waste measurement solutions obstructs domain experts from guiding policy towards sustainable food resource management. We propose a system for measuring household food waste using an AI-enabled compost bin. Food waste identification can be framed as a computer vision task, however no public datasets of labeled post-consumer food items have been released to date. To power the development of computer vision models for food waste identification, we design a compost bin equipped with imaging sensors capable of capturing 2D, 3D, and thermal information about discarded food. This device encourages sustainable composting practices while building a novel dataset of commingled food waste images annotated with descriptive labels and segmentation masks. We design a volunteer-driven study to deploy fifty of these devices in households across the state of Oregon.

![Bin](/images/bin_partial_open.jpg){:width="60%"}

Our research has three primary objectives:

1. We design and manufacture the Smart Compost Bin, a low-cost AI-enabled device which
automatically collects image and sensor data for each disposed food item.

2. To produce the first annotated, public image dataset of post-consumer food, we will conduct a
pilot study with fifty households to annotate images of food waste using our companion iOS/Android app.

3. We will use our dataset to train a computer vision model to automatically measure household
food waste by segmenting disposed items from images of commingled food refuse

![Example Image](/images/compost_segmented.jpg)

![System Diagram](/images/cloud_pipeline_v4.png){:width="85%"}

You can see our first publication, describing the design and implementation of the Smart Compost Bin
[here](https://aidanbeery.com/files/cofi_2024.pdf). 

This work was supervised by [Dr. 
Patrick Donnelly](https://engineering.oregonstate.edu/people/patrick-donnelly) at [Soundbendor Lab](https://soundbendor.org/), Oregon State University.

Sponsored by the [Foundation for Food and Agriculture Research](https://foundationfar.org/) and [Kroger Zero Hunger Zero Waste
Foundation](https://thekrogercozerohungerzerowastefoundation.com/).

![App Screenshots](/images/app_screenshots.png)

![SCB Sensors](/images/scb_sensors.png)


