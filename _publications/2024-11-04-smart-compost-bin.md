---
title: "Smart Compost Bin for Measurement of Consumer Food Waste"
collection: publications
permalink: /publication/2024-11-04-smart-compost-bin
excerpt: 'We present the Smart Compost Bin, a novel food waste measurement device. Our low-cost 3D printed compost bin allows household users to gain insights on their food waste and compost habits, using a camera and environmental sensors to automatically classify and quantify food disposals. Using this device, we propose a pilot study to leverage volunteer households to annotate food waste images taken from our device, enabling the development of a robust food waste image segmentation model.'
date: 2024-11-04
venue: 'CoFI 2024'
paperurl: 'http://aidan-b1409.github.io/files/cofi_2024.pdf'
#citation: ''
---
The rising amounts of food waste across the world is a severe environmental, social, and economic catastrophe. The majority of food waste occurs at the consumer level, yet we have no reliable means to quantify this waste. A lack of publicly available image datasets of commingled food waste has prohibited researchers from leveraging advances in computer vision for the task of automatic food waste measurement. We present an AI-assisted compost bin that automatically measures kitchen compost waste by collecting 2D, 3D, and thermal images alongside measurements of temperature, humidity, pressure, and volatile organic compounds. The compost bin utilizes speech recognition technology that allows users to verbally describe the items they deposit. We provide a companion mobile app that tasks a subset of volunteer users to draw boundaries around individual discarded food items in order to generate high-quality segmentation masks of food items present in the image. We will deploy this device in a forthcoming field study to curate a large and novel dataset of commingled food waste. This dataset will enable computer vision researchers to train intelligent models capable of quantifying and measuring food waste without the need of costly, labor-intensive human subject studies. Additionally, we train a preliminary food image segmentation model using existing datasets of images of uneaten food items, and evaluate it on images taken by our compost bin to demonstrate the critical need for a large, high-quality dataset of commingled compost waste.

[Download paper here](http://academicpages.github.io/files/paper2.pdf)

Recommended citation: Aidan J. Beery, Daniel W. Eastman, Jake Enos, William Richards, and Patrick J. Donnelly. 2024. Smart Compost Bin for Measurement of Consumer Food Waste. In Companion Proceedings of the 26th International Conference on Multimodal Interaction (ICMI Companion '24). Association for Computing Machinery, New York, NY, USA, 100–107. https://doi.org/10.1145/3686215.3686216
