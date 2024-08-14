<div align="center">

# Generative AI Examples

[![version](https://img.shields.io/badge/release-0.8-green)](https://github.com/opea-project/GenAIExamples/releases)
[![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/neural-compressor/blob/master/LICENSE)

---

<div align="left">

## Introduction

GenAIComps-based Generative AI examples offer streamlined deployment, testing, and scalability. All examples are fully compatible with Docker and Kubernetes, supporting a wide range of hardware platforms such as Gaudi, Xeon, and other hardwares.

## Architecture

[GenAIComps](https://github.com/opea-project/GenAIComps) is a service-based tool that includes microservice components such as llm, embedding, reranking, and so on. Using these components, various examples in GenAIExample can be constructed, including ChatQnA, DocSum, etc.

[GenAIInfra](https://github.com/opea-project/GenAIInfra), part of the OPEA containerization and cloud-native suite, enables quick and efficient deployment of GenAIExamples in the cloud.

[GenAIEval](https://github.com/opea-project/GenAIEval) measures service performance metrics such as throughput, latency, and accuracy for GenAIExamples. This feature helps users compare performance across various hardware configurations easily.

## Getting Started

GenAIExamples offers flexible deployment options that cater to different user needs, enabling efficient use and deployment in various environments. Here’s a brief overview of the three primary methods: Python startup, Docker Compose, and Kubernetes.

1. <b>Docker Compose</b>: Check the released docker images in [docker image list](./docker_images_list.md) for detailed information.
2. <b>Kubernetes</b>: Follow the steps at [K8s Install](https://github.com/opea-project/docs/tree/main/guide/installation/k8s_install) and [GMC Install](/guide/installation/gmc_install/gmc_install.md) to setup k8s and GenAI environment .

Users can choose the most suitable approach based on ease of setup, scalability needs, and the environment in which they are operating.

### Deployment

<table>
    <tr>
        <th rowspan="3" style="text-align:center;">Use Cases</th>
        <th colspan="4" style="text-align:center;">Deployment</th>
    </tr>
    <tr>
        <td colspan="2" style="text-align:center;">Docker Compose</td>
        <td rowspan="2" style="text-align:center;">Kubernetes</td>
    </tr>
    <tr>
        <td style="text-align:center;">Xeon</td>
        <td style="text-align:center;">Gaudi</td>
    </tr>
    <tr>
        <td style="text-align:center;">ChatQnA</td>
        <td><a href="/GenAIExamples/ChatQnA/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/ChatQnA/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/ChatQnA/kubernetes/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">CodeGen</td>
        <td><a href="/GenAIExamples/CodeGen/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/CodeGen/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/CodeGen/kubernetes/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">CodeTrans</td>
        <td><a href="/GenAIExamples/CodeTrans/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/CodeTrans/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/CodeTrans/kubernetes/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">DocSum</td>
        <td><a href="/GenAIExamples/DocSum/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/DocSum/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/DocSum/kubernetes/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">SearchQnA</td>
        <td><a href="/GenAIExamples/SearchQnA/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/SearchQnA/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/SearchQnA/kubernetes/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">FaqGen</td>
        <td><a href="/GenAIExamples/FaqGen/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/FaqGen/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="/GenAIExamples/FaqGen/kubernetes/manifests/README.md">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">Translation</td>
        <td><a href="/GenAIExamples/Translation/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/Translation/docker/gaudi/README.md">Gaudi Link</a></td>
        <td><a href="https://github.com/opea-project/GenAIExamples/tree/main/Translation/kubernetes">K8s Link</a></td>
    </tr>
    <tr>
        <td style="text-align:center;">AudioQnA</td>
        <td><a href="/GenAIExamples/AudioQnA/docker/xeon/README.md">Xeon Link</a></td>
        <td><a href="/GenAIExamples/AudioQnA/docker/gaudi/README.md">Gaudi Link</a></td>
        <td>Not supported yet</td>
    </tr>
    <tr>
        <td style="text-align:center;">VisualQnA</td>
        <td><a href="https://github.com/opea-project/GenAIExamples/tree/main/VisualQnA">Xeon Link</a></td>
        <td><a href="https://github.com/opea-project/GenAIExamples/tree/main/VisualQnA">Gaudi Link</a></td>
        <td>Not supported yet</td>
    </tr>
</table>

## Support Examples

Check [here](./supported_examples.md) for detailed information of supported examples, models, hardwares, etc.

## Additional Content

- [Code of Conduct](/community/CODE_OF_CONDUCT.md)
- [Contribution](/community/CONTRIBUTING.md)
- [Security Policy](/community/SECURITY.md)
- [Legal Information](/LEGAL_INFORMATION.md)
