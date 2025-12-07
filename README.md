# Elasticsearch Rank Eval
## Contents
1.  [Summary](#summary)
2.  [Architecture](#architecture)
3.  [Features](#features)
4.  [Prerequisites](#prerequisites)
5.  [Installation](#installation)
6.  [Usage](#usage)

## Summary <a name="summary"></a>
This is a demonstration of usage of Elastic rank evaluations using synthetic data and judgment sets.

## Architecture <a name="architecture"></a>
![architecture](assets/highlevel.png) 


## Features <a name="features"></a>
- Jupyter notebook
- Builds an Elastic Serverless deployment via Terraform
- Generates a document and judgment set via LLM (Gemini 3)
- Creates a Jina.ai reranker inference endpoint
- Creates various query strategies (lexical, semantic, hybrid, etc) for evaluation
- Executes relevance evaluations on the given document, judgment, and eval sets.
- Deletes the entire deployment via Terraform

## Prerequisites <a name="prerequisites"></a>
- terraform
- Elastic Cloud account and API key
- Jina.ai API key
- Gemini API key
- Python

## Installation <a name="installation"></a>
- Edit the terraform.tfvars.sample and rename to terraform.tfvars
- Create a Python virtual environment

## Usage <a name="usage"></a>
- Execute notebook