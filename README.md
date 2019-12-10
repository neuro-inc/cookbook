# Welcome to ML Cookbook

What you will find here is a curated collection of ML Recipes: ready-to-use examples, best practices, and learning materials available to you in the form of interactive environments that run on Neuro Platform.

Using ML Recipes, you can:

* Run state of the art (SOTA) deep learning models for a variety of applied tasks.
* Interact with the results and extend the solution.
* Upload data and download the results using a desktop or mobile device.
* Make your experiments reproducible.

You have two options of how you might wish to use our recipes. You can sign up as [free tier user](https://neu.ro/) and experiment with the recipes within our managed installation of the platform. You can also install Neuro into your AWS, GCP, or Azure cloud account or on-perm GPU rack and use the recipes there.

## What's Inside?

### Vision

* [Object detection](https://github.com/neuromation/ml-recipe-object-detection). An end to end object detection pipeline for objects represented in the [Common Objects in Context (COCO)](http://cocodataset.org) dataset that allows you to evaluate performance on real life images and to add new object classes.

### Language

* [Language Recipes](https://github.com/neuromation/ml-recipe-nlp). Based on [Microsoft's NLP Notebooks](https://github.com/microsoft/nlp), these let you start building Natural Language Processing systems for various scenarios, such as: Topic Classification, Named Entity Recognition, Question Answering, Sentence Similarity, and more.

* [Hierarchical Attention](https://github.com/neuromation/ml-recipe-hier-attention). Based on highly cited paper [Hierarchical Attention Networks for Document Classification](https://arxiv.org/abs/1608.07775) (Z. Yang et al.), published in 2017, this recipe demonstrates how to apply this two-step architecture to sentiment classification.

### Learning

* [Practical Deep Learning for Coders, v3](https://github.com/neuromation/ml-recipe-course-fast-ai-v3). Brought to you by [fast.ai](https://fast.ai), this course aims to make deep learning more comfortable to use, thereby getting more people from all backgrounds involved.

* [A Code-First Introduction to Natural Language Processing](https://github.com/neuromation/ml-recipe-course-fast-ai-nlp) is another great [course](https://www.fast.ai/2019/07/08/fastai-nlp/) from fast.ai. It covers a lot of ground, including transfer learning for NLP, tips on working with languages other than English, attention and the transformer, text generation algorithms, and issues of bias.

## Prerequisites

* Familiarity with working with data in Python.
* Familiarity with machine learning concepts (such as training and test sets).
* Some experience with PyTorch and neural networks is helpful.

## Getting Started

### Install the Neuro CLI

To work with ML Recipes, you need to install the Neuro Platform CLI.

```shell
pip install -U neuromation
neuro login
```

Paste the above in a macOS, Windows, or Linux terminal prompt. This command automatically installs the Neuro CLI and brings you to the login screen of Neuro Platform.

The Neuro Platform CLI requires Python 3.7 to be installed. We suggest installing Anaconda Python 3.7 Distribution. On some distributions, you might have to run `pip3 install -U neuromation`.

### Run ML Recipe

Choose an ML Recipe from the list above, clone the corresponding repository and follow the instructions from that recipe's README.
