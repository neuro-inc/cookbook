# Welcome to ML Cookbook

Here is a curated collection of ML Recipes: ready-to-use examples, best practices, and learning materials available to you in the form of interactive environments running on [Neuro Platform](https://neu.ro).

With ML Recipes, you can:

* Run state of the art (SOTA) deep learning models for a variety of applied tasks.
* Interact with the results and extend the solution.
* Upload data, download the results using desktop or mobile device.
* Make your experiments reproducible.

You can start by taking one of these recipes and experimenting with it as a [free tier user](https://neu.ro/) or by installing Neuro into your AWS, GCP, or Azure cloud account or on-prem GPU rack.

## What's Inside?

### Vision

* [Object detection](https://github.com/neuromation/ml-recipe-object-detection) - end to end object detection pipeline for objects represented in [Common Objects in Context (COCO)](http://cocodataset.org) dataset. Allows to evaluate performance on real-life images and add new object classes.

### Language

* [NLP](https://github.com/neuromation/ml-recipe-nlp) - based on [Microsoft's NLP Notebooks](https://github.com/microsoft/nlp). Start building Natural Language Processing systems for the following scenarios: Topic Classification, Named Entity Recognition, Question Answering, Sentence Similarity, and more.

### Learn

* [Practical Deep Learning for Coders, v3](https://github.com/neuromation/ml-recipe-course-fast-ai-v3) - brought to you by [fast.ai](https://fast.ai) aiming to make deep learning more comfortable to use and getting more people from all backgrounds involved.

* [A Code-First Introduction to Natural Language Processing](https://github.com/neuromation/ml-recipe-course-fast-ai-nlp) - everything you need to follow [the NLP from fast.ai](https://www.fast.ai/2019/07/08/fastai-nlp/) including transfer learning for NLP, tips on working with languages other than English, attention and the transformer, text generation algorithms, issues of bias and some steps towards addressing them.

## Prerequisites

* Familiarity with working with data in Python.
* Machine learning concepts (such as training and test sets).
* Some experience with PyTorch and neural networks is helpful.

## Getting Started

### Install Neuro CLI 

To work with ML Recipes, you need to install Neuro Platform CLI.

```shell
pip install -U neuromation
neuro login
```

Paste that in a macOS, Windows, or Linux terminal prompt. This command automatically installs Neuro CLI and brings you to the log you in screen of Neuro Platform.

Neuro Platform CLI requires Python 3.7 installed. We suggest installing Anaconda Python 3.7 Distribution. On some distributions, you might have to run `pip3 install -U neuromation`.

### Run ML Recipe

Choose an ML Recipe from the list above, clone the corresponding repository and follow the instructions
 from that recipe's README.
