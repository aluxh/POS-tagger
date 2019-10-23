## Introduction

In this notebook, I've used the [Pomegranate](https://github.com/jmschrei/pomegranate) library to build a hidden Markov model for part of speech tagging with a [universal tagset](http://www.petrovi.de/data/universal.pdf). 

**Hidden Markov models** have been able to achieve >96% tag accuracy with larger tagsets on realistic text corpora. Hidden Markov models have also been used for speech recognition and speech generation, machine translation, gene recognition for bioinformatics, and human gesture recognition for computer vision, and more.

This notebook was provided as a template from **Udacity's Natural Language Processing Nanodegree** for implementation. And, I've added new functionalities in those sections that begins with **'IMPLEMENTATION'** in the header.

## Getting Started

If you're planning to download and run the codes writte in the Jupyter notebook, you can first download a copy of this [project](https://github.com/aluxh/POS-tagger), then run a Jupyter server locally with [Anaconda](https://www.anaconda.com/download/).

1. Open a terminal and clone the project repository:
```
$ git clone https://github.com/aluxh/POS-tagger
```

3. Switch to the project folder and create a conda environment (note: you must already have Anaconda installed):
```
$ cd hmm-tagger
hmm-tagger/ $ conda env create -f hmm-tagger.yaml
```

4. Activate the conda environment, then run the jupyter notebook server. (Note: windows users should run `activate hmm-tagger`)
```
hmm-tagger/ $ source activate hmm-tagger
(hmm-tagger) hmm-tagger/ $ jupyter notebook
```

Depending on your system settings, Jupyter will either open a browser window, or the terminal will print a URL with a security token. If the terminal prints a URL, simply copy the URL and paste it into a browser window to load the Jupyter browser. Once you load the Jupyter browser, select the project notebook (HMM tagger.ipynb) and view the implementation of the HMM POS tagger.