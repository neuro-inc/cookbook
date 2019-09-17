# fast.ai NLP Course

Interactive development environment to get you up and running with [fast.ai NLP Course](https://www.fast.ai/2019/07/08/fastai-nlp/) [notebooks](https://github.com/fastai/course-nlp)

# Development Environment

This project is designed to run on [Neuro Platform](https://neu.ro), so you can jump into problem-solving right away.

## Directory Structure

| Mount Point              | Description                       | Storage URI                     |
|:------------------------ |:--------------------------------- |:------------------------------- |
|`/project/data/`          | Test data                         | `storage:course-fastai-nlp/data/`         |
|`/project/modules/`       | Python modules                    | `storage:course-fastai-nlp/modules/`      |
|`/project/notebooks/`     | Jupyter notebooks                 | `storage:course-fastai-nlp/notebooks/`    |
|`/project/results/`       | Logs and results                  | `storage:course-fastai-nlp/results/`      |


## Development

Follow the instructions below to setup the environment and start Jupyter development session backed by CPU or GPU.

### Neuro Platform

* Setup development environment `make setup`
* Run Jupyter with GPU: `make jupyter`
* TBD: Run Jupyter with CPU: `make jupyter-cpu`
* Kill Jupyter: `make kill_jupyter`

# Data

### Uploading via Web UI

From local machine run `make filebrowser` and open job's URL from your mobile device or desktop. Through a simple file explorer interface you can upload test images and perform file operations.

### Uploading via CLI

From local machine run `make upload_data`. This will push local files stored in `./data` into `storage:course-fastai-nlp/data` mounted to your development environment's `/project/data`.# course-fastai-nlp
