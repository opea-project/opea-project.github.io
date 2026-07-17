# RFC: Data Catalog Service

This RFC Proposes an Apache Gravitino microservice to act as a lakehouse connector for OPEA applications to integrate with.  

## Author(s)

[Lisa N. Cao](https://github.com/lisancao/)

## Status

`Under Review` 

## Objective

OPEA's applications, even mature ones such as ChatQ&A are difficult to set up due to the complexity of the project, but also because enterprise organizations have a hard time consolidating all their data they want to train on in one place. Currently data sources have to be manually connected to OPEA applications and managed separately, which creates a barrier for governance. Apache Gravitino can provide data management, tagging, and access controls for OPEA applications and agentic workflows that will act as guardrails to source data make the OPEA applications appropriate for enterprise and production use case, but also provide a standard set of APIs for lineage, lifecycle management, and data discovery. 

## Motivation

Apache Gravitino's metastore model is designed for enterprise and AI use cases, making it the ideal fit for the project. Coupled with Gravitino's MCP server andflexible deployment options, it will be a good choice for an interface for OPEA applications to access source data safely. 

## Design Proposal

Deploy Gravitino as a catalog microservice that is meant to service the Generative AI Components (GenAIComps), with a focus on Langchain and LlamaIndex Framework support. This can generally be done using a Gravitino server and leveraging the Python client, but requires that the user sets up Gravitino on their end. Perhaps it can be integrated with the Dataprep and guardrails. 


## Alternatives Considered

N/A

## Compatibility

list possible incompatible interface or workflow changes if exists.

## Miscellaneous

- Performance Impact, such as speed, memory, accuracy.
- Engineering Impact, such as binary size, startup time, build time, test times.
- Security Impact, such as code vulnerability.
- TODO List or staging plan.
