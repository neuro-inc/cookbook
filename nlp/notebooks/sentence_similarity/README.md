# Sentence Similarity

This folder contains examples and best practices, written in Jupyter notebooks, for building
sentence similarity models. The [gensen](../../utils_nlp/models/gensen) and [pretrained
embeddings](../../utils_nlp/models/pretrained_embeddings) utility scripts are used to speed up the
model building process in the notebooks.  
The sentence similarity scores can be used in a wide
variety of applications, such as search/retrieval, nearest-neighbor or kernel-based classification
methods, recommendations, and ranking tasks.

## What is sentence similarity

Sentence similarity or semantic textual similarity is a measure of how similar two pieces of text
are, or to what degree they express the same meaning. Related tasks include paraphrase or duplicate
identification, search, and matching applications. The common methods used for text similarity range
from simple word-vector dot products to pairwise classification, and more recently, deep neural
networks.

Sentence similarity is normally calculated by the following two steps:

1. obtaining the embeddings of the sentences

2. taking the cosine similarity between them as shown in the following figure([source](https://tfhub.dev/google/universal-sentence-encoder/1)):

    ![Sentence Similarity](https://nlpbp.blob.core.windows.net/images/example-similarity.png)

## Summary

|Notebook|Description|Dataset|
|---|---|---|
|[Creating a Baseline model](baseline_deep_dive.ipynb)| A baseline model is a basic solution that serves as a point of reference for comparing other models to. The baseline model's performance gives us an indication of how much better our models can perform relative to a naive approach.|[STS Benchmark](http://ixa2.si.ehu.es/stswiki/index.php/STSbenchmark#STS_benchmark_dataset_and_companion_dataset)|
|[BERT Sentence Encoder](bert_encoder.ipynb)|In this notebook, we show how to extract features from pretrained BERT as sentence embeddings.|Handcrafted sample data|
