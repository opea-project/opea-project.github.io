# Code Translation Application

Code translation is the process of converting code written in one programming language to another programming language while maintaining the same functionality. This process is also known as code conversion, source-to-source translation, or transpilation. Code translation is often performed when developers want to take advantage of new programming languages, improve code performance, or maintain legacy systems. Some common examples include translating code from Python to Java, or from JavaScript to TypeScript.

## Table of Contents

1. [Architecture](#architecture)
2. [Deployment Options](#deployment-options)
3. [Monitoring and Tracing](./README_miscellaneous.md)

## Architecture

The CodeTrans application is an end-to-end workflow that leverages the capability of LLMs. The workflow falls into the following architecture:

![architecture](./assets/img/code_trans_architecture.png)

The CodeTrans example is implemented using the component-level microservices defined in [GenAIComps](https://github.com/opea-project/GenAIComps).

This Code Translation use case demonstrates Text Generation Inference across multiple platforms. Currently, we provide examples for [Intel Gaudi2](https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi-overview.html) and [Intel Xeon Scalable Processors](https://www.intel.com/content/www/us/en/products/details/processors/xeon.html), and we invite contributions from other hardware vendors to expand OPEA ecosystem.

## Deployment Options

The table below lists currently available deployment options. They outline in detail the implementation of this example on selected hardware.

| Category               | Deployment Option    | Description                                                                 |
| ---------------------- | -------------------- | --------------------------------------------------------------------------- |
| On-premise Deployments | Docker compose       | [CodeTrans deployment on Xeon](./docker_compose/intel/cpu/xeon/README.md)   |
|                        |                      | [CodeTrans deployment on Gaudi](./docker_compose/intel/hpu/gaudi/README.md) |
|                        |                      | [CodeTrans deployment on AMD ROCm](./docker_compose/amd/gpu/rocm/README.md) |
|                        | Kubernetes           | [Helm Charts](./kubernetes/helm/README.md)                                  |
|                        | Azure                | Work-in-progress                                                            |
|                        | Intel Tiber AI Cloud | Work-in-progress                                                            |

## Validated Configurations

| **Deploy Method** | **LLM Engine** | **LLM Model**                      | **Hardware** |
| ----------------- | -------------- | ---------------------------------- | ------------ |
| Docker Compose    | vLLM, TGI      | mistralai/Mistral-7B-Instruct-v0.3 | Intel Gaudi  |
| Docker Compose    | vLLM, TGI      | mistralai/Mistral-7B-Instruct-v0.3 | Intel Xeon   |
| Docker Compose    | vLLM, TGI      | Qwen/Qwen2.5-Coder-7B-Instruct     | AMD ROCm     |
| Helm Charts       | vLLM, TGI      | mistralai/Mistral-7B-Instruct-v0.3 | Intel Gaudi  |
| Helm Charts       | vLLM, TGI      | mistralai/Mistral-7B-Instruct-v0.3 | Intel Xeon   |
| Helm Charts       | vLLM, TGI      | mistralai/Mistral-7B-Instruct-v0.3 | AMD ROCm     |
