---
title: "Nonnegative Matrix Factorization for Percussion Audio Separation"
excerpt: "Applying NMF to extract source audio components for mixed percussion samples"
collection: portfolio
---

We present some supplementary material, including extracted audio for accelerated hierarchical least-squares NMF for
audio source separation.

# Sample - Amen Break
## Original Audio
{% include embed-audio.html src="/assets/audio/runningExample_AmenBreak.wav" %}

![Spectogram 1](/assets/img/amenbreak_spectogram.png)

## Sources

- Kick Drum
{% include embed-audio.html src="/assets/audio/amenbreak_sample0.wav" %}

- Snare Drum
{% include embed-audio.html src="/assets/audio/amenbreak_sample1.wav" %}

- Hi-Hat
{% include embed-audio.html src="/assets/audio/amenbreak_sample2.wav" %}

![Source 1](/assets/img/amenbreak_source0.png){:width="32%"}![Source 2](/assets/img/amenbreak_source1.png){:width="32%"}![Source 3](/assets/img/amenbreak_source2.png){:width="32%"}


# Sample - 808
## Original Audio
{% include embed-audio.html src="/assets/audio/runningExample_808Mixture.wav" %}
![Spectogram 2](/assets/img/808_spectogram.png)

## Sources

- Cymbal
{% include embed-audio.html src="/assets/audio/808_sample0.wav" %}

- Snare
{% include embed-audio.html src="/assets/audio/808_sample1.wav" %}

- Bass
{% include embed-audio.html src="/assets/audio/808_sample2.wav" %}

![Source 1](/assets/img/808_source0.png){:width="32%"}![Source 2](/assets/img/808_source1.png){:width="32%"}![Source 3](/assets/img/808_source2.png){:width="32%"}


# Sample - Funky
## Original Audio
{% include embed-audio.html src="/assets/audio/runningExample_FunkyMixture.wav" %}
![Spectogram 3](/assets/img/funky_spectogram.png)

## Sources

- Kick Drum
{% include embed-audio.html src="/assets/audio/funky_sample0.wav" %}

- Mid Tom
{% include embed-audio.html src="/assets/audio/funky_sample1.wav" %}

- Hi-Hat
{% include embed-audio.html src="/assets/audio/funky_sample2.wav" %}

![Source 1](/assets/img/funky_source0.png){:width="32%"}![Source 2](/assets/img/funky_source1.png){:width="32%"}![Source 3](/assets/img/funky_source2.png){:width="32%"}

# Sample - I Got You
## Original Audio
{% include embed-audio.html src="/assets/audio/runningExample_IGotYouMixture.wav" %}
![Spectogram 4](/assets/img/igotyou_spectogram.png)

## Sources

- Kick Drum
{% include embed-audio.html src="/assets/audio/igotyou_sample0.wav" %}

- Snare Drum
{% include embed-audio.html src="/assets/audio/igotyou_sample1.wav" %}

- Brass
{% include embed-audio.html src="/assets/audio/igotyou_sample2.wav" %}


![Source 1](/assets/img/igotyou_source0.png){:width="32%"}![Source 2](/assets/img/igotyou_source1.png){:width="32%"}![Source 3](/assets/img/igotyou_source2.png){:width="32%"}

You can see the code for this experiment [here](https://github.com/Aidan-B1409/AccelSepNMF). For more details, find my
report [here](/files/Beery_A_AI568FinalReport.pdf)

This project was completed as part of the requirements for AI-586 Applied Matrix Analysis at OSU.
