# Welcome to AI Kits

This is a curated collection of learning materials, ready-to-use examples and best practices available to you in the form of interactive environments running on [Neuro Platform](https://neu.ro).

With AI kits you can:
* Run state of the art (SoTA) deep learning models for a variety of applied tasks.
* Interact with the results and extend the solution.
* Upload data, download the results using desktop or mobile device.
* Make your experiments reproducible.

You can start by taking one of these kits and experimenting with it as a [free tier user](https://neu.ro/) or by installing Neuro into your AWS, GCP or Azure cloud account or on-prem GPU rack.

## What's Inside?

### Learn

* [Practical Deep Learning for Coders, v3](course-fast-ai-v3) - brought to you by [fast.ai](https://fast.ai) aiming to make deep learning easier to use and getting more people from all backgrounds involved.

### Vision

* [Object detection](object-detection) - end to end object detection pipeline for objects represented in [Common Objects in Context (COCO)](http://cocodataset.org) dataset. Allows to  evaluate performance on real life images and add new object classes.

* [Face Recognition](face-recognition) - validate claimed identity or identify a person based on the image of a face. Add new identities and test on real life images.

### Language

* [A Code-First Introduction to Natural Language Processing](course-fast-ai-nlp) - everything you need to follow [the NLP from fast.ai](https://www.fast.ai/2019/07/08/fastai-nlp/) including transfer learning for NLP, tips on working with languages other than English, attention and the transformer, text generation algorithms, issues of bias and some steps towards addressing them.

* [Microsoft's NLP Notebooks](microsoft-nlp) - start building Natural Language Processing systems for the following scenarios: Topic Classification, Named Entity Recognition, Question Answering, Sentence Similarity and more.

* [PyTorch-Transformers](hugging-face-pytorch-transformers) - state-of-the-art pre-trained models for Natural Language Processing (NLP).

## Prerequisites

* Familiarity with working with data in Python.
* Machine learning concepts (such as training and test sets).
* Some experience with PyTorch and neural networks is helpful.

## Getting Started

### Clone the Repository

```
git clone --recursive https://github.com/neuromation/ai-kits.git
```

Make sure to use `--recursive` argument to get a full copy of repositories included in the AI Kits.


### Install Neuro CLI

To work with AI Kits you need to install `neuro` CLI client.

Neuro CLI requires Python 3.7. We suggest installing Anaconda Python 3.7 Distribution. On some distributions you might have to run pip3 install -U neuromation.

```shell
pip install -U neuromation
neuro login
```

Paste that in a macOS, Windows or Linux terminal prompt. This will automatically install Neuro CLI and initiate login flow.

### Setup and Run AI Kit

* Navigate to the kit of interest: `cd ai-kits/course-fast-ai-nlp`
* Setup the environment: `make setup`
* Run Jupyter notebook: `make jupyter`
