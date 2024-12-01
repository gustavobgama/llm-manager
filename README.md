# Introduction

Ollama LLM manager and an interface to interact with it based on OpenWebUI.

# Installation

## Pre Requisites

### Required

* [Docker](https://docs.docker.com/engine/install/)
* [Docker Compose](https://docs.docker.com/compose/install/)

### Optional

* [Nvidia Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#installation)

## Steps

1. Clone the repository:

```sh
git clone https://github.com/gustavobgama/llm-manager.git
```

2. Navigate to the project directory:

```sh
cd llm-manager
```

3. Start the manager:

```sh
docker compose up -d
```

All ollama cli commands are available with:

```sh
docker compose exec ollama ollama --help
```

For instance, you can download a new model:

```sh
docker compose exec ollama ollama pull llama3.2
```

You can also visit the web interface [here](http://localhost:8080) to interact with downloaded models.

# References

* Ollama documentation: https://ollama.com/
* OpenWebUI documentation: https://docs.openwebui.com/