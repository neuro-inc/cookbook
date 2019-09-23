# Language Kit

This kit is a subset of [Microsoft's NLP Notebooks](https://github.com/microsoft/nlp) and aims to present most common scenarios with the focus on deep learning and portability across cloud providers.

|Category|Applications|Methods|Languages|
|---| ------------------------ | ------------------- |---|
|[Text Classification](text_classification)|Topic Classification|BERT, XLNet|en, hi, ar|
|[Named Entity Recognition](named_entity_recognition) |Wikipedia NER|BERT|en|
|[Entailment](entailment)|MultiNLI Natural Language Inference|BERT|en|
|[Sentence Similarity](sentence_similarity)|STS Benchmark|Representation: TF-IDF, Word Embeddings, Doc Embeddings<br>Metrics: Cosine Similarity, Word Mover's Distance<br> Models: BERT||
|[Embeddings](embeddings)|Custom Embeddings Training|Word2Vec, fastText, GloVe||
|[Model Explainability](model_explainability)|DNN Layer Explanation|DUUDNM (Guan et al.)|

# Development Environment

This project is designed to run on [Neuro Platform](https://neu.ro), so you can jump into problem-solving right away. Follow the instructions below to setup the environment and start Jupyter development session backed by GPU.

## Neuro Platform

* Setup development environment `make setup`
* Run Jupyter with GPU: `make jupyter`
* Kill Jupyter: `make kill_jupyter`

# Data

## Uploading via Web UI

From local machine run `make filebrowser` and open job's URL from your mobile device or desktop. Through a simple file explorer interface you can upload test images and perform file operations.

## Uploading via CLI

From local machine run `make upload_data`. This will push local files stored in `./data` into `storage:nlp/data` mounted to your development environment's `/project/data`.
