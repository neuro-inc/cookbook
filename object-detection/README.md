# Object Detection

End to end object detection pipeline for objects represented in [Common Objects in Context (COCO)](http://cocodataset.org) dataset. Allows to  evaluate performance on real life images and add new object classes.

# Development Environment

This project is designed to run on [Neuro Platform](https://neu.ro), so you can jump into problem-solving right away.

## Directory Structure

| Mount Point              | Description                       | Storage URI                     |
|:------------------------ |:--------------------------------- |:------------------------------- |
|`/project/data/`          | Test images                       | `storage:detection-kit/data/`         |
|`/project/detection_kit/` | Python modules                    | `storage:detection-kit/detection_kit/`      |
|`/project/notebooks/`     | Jupyter notebooks                 | `storage:detection-kit/notebooks/`    |
|`/project/results/`       | Logs and results                  | `storage:detection-kit/results/`      |


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

From local machine run `make upload_data`. This will push local files stored in `./data` into `storage:detection-kit/data` mounted to your development environment's `/project/data`.
