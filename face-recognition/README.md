# Face Recognition Kit: Identification and Verification (Authentication)


## Face Verification

Face verification is concerned with validating a claimed identity based on the image of a face, and either accepting or rejecting the identity claim (one-to-one matching).

## Face Identification

Face identification is concerned with identifying a person based on the image of a face. This face image has to be compared with all the registered persons (one-to-many matching).

# Development Environment

This project is designed to run on [Neuro Platform](https://neu.ro), so you can jump into problem-solving right away.

## Directory Structure

| Mount Point              | Description                       | Storage URI                     |
|:------------------------ |:--------------------------------- |:------------------------------- |
|`/project/data/`          | Identities and test images        | `storage:face-id/data/`         |
|`/project/face-id/`       | Python modules                    | `storage:face-id/face-id/`      |
|`/project/notebooks/`     | Jupyter notebooks                 | `storage:face-id/notebooks/`    |
|`/project/requirements/`  | pip and apt-get packages required | `storage:face-id/requirements/` |
|`/project/results/`       | Logs and results                  | `storage:face-id/results/`      |


## Development

Follow the instructions below to setup the environment and start Jupyter development session backed by CPU or GPU.

### Neuro Platform

* Setup development environment `make setup`
* Run Jupyter with GPU: `make jupyter`
* TBD: Run Jupyter with CPU: `make jupyter-cpu`
* Kill Jupyter: `make kill_jupyter`


### Developing Locally

```shell
docker run \
    -p 8888:8888 \
    -v $(pwd)/data:/project/data \
    -v $(pwd)/code:/project/code \
    -v $(pwd)/notebooks:/project/notebooks \
    -v $(pwd)/results:/project/results \
    neuromation/base \
    'jupyter notebook --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir=/project/notebooks'
```

## Data

### Directory Structure

Identities and test images are stored in `/data` with the following structure:

```
/identities
    /alice
        /alice1.jpg
        /alice2.jpg
        ...
    /bob
        /bob1.jpg
        /bob2.jpg
        ...
    /test
        face1.jpg
        face2.jpg
        ...
```

### Uploading via Web UI

Run `make filebrowser` and open job's URL. After that you can add and update identities through simple file operations via shared URL accessible from desktop and mobile devices.

### Uploading via CLI

If you prefer to maintain identity structure locally and replicate it remotely, you can do in `/data` directory and sync with Neuro Platform file storage by running `make upload_data`