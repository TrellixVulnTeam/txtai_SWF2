# Installation

![install](images/install.png#only-light)
![install](images/install-dark.png#only-dark)

The easiest way to install is via pip and PyPI

```
pip install txtai
```

Python 3.7+ is supported. Using a Python [virtual environment](https://docs.python.org/3/library/venv.html) is recommended.

## Optional dependencies

txtai has the following optional dependencies that can be installed as extras. The patterns below are supported
in setup.py install_requires sections.

_Note: Extras are provided for convenience. Alternatively, individual packages can be installed to limit dependencies._

### All

Install all dependencies.

```
pip install txtai[all]
```

### API

Serve txtai via a web API.

```
pip install txtai[api]
```

### Cloud

Interface with cloud compute.

```
pip install txtai[cloud]
```

### Console

Command line index query console.

```
pip install txtai[console]
```

### Database

Additional content storage options.

```
pip install txtai[database]
```

### Graph

Topic modeling, data connectivity and network analysis.

```
pip install txtai[graph]
```

### Model

Additional non-standard models.

```
pip install txtai[model]
```

### Pipeline

All pipelines - default install comes with most common pipelines.

```
pip install txtai[pipeline]
```

### Similarity

Word vectors, support for sentence-transformers models not on the HF Hub and additional ANN libraries.

```
pip install txtai[similarity]
```

### Workflow

All workflow tasks - default install comes with most common workflow tasks.

```
pip install txtai[workflow]
```

Multiple dependencies can be specified at the same time.

```
pip install txtai[pipeline,workflow]
```

## Environment specific prerequisites

Additional environment specific prerequisites are below.

### Linux

Optional audio transcription requires a [system library to be installed](https://github.com/bastibe/python-soundfile#installation)

### macOS

Run `brew install libomp` see [this link](https://github.com/kyamagu/faiss-wheels#prerequisite)

_Note: Older versions of Python had issues with PyTorch 1.12+. If issues are encountered, either upgrade Python or downgrade PyTorch._

### Windows

Optional dependencies require [C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

_Note: Older versions of Python did not have SQLite JSON support. If issues are encountered, upgrade to a later version of Python._

The [txtai build workflow](https://github.com/neuml/txtai/blob/master/.github/workflows/build.yml) occasionally has work arounds for other known but temporary dependency issues.

## Install from source

txtai can also be installed directly from GitHub to access the latest, unreleased features.

    pip install git+https://github.com/neuml/txtai

## Run with containers

Docker images are available for txtai. [See this section](../cloud) for more information on container-based installs.
