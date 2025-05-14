# Module 1: Introduction to Open-Source AI and LLMs

Welcome to Module 1 of the Open Source LLM Zoomcamp! In this module, we'll explore how to run and deploy these powerful models using AMD GPUs and modern cloud infrastructure.

* Video Link (Coming Soon)
* Slides (Coming Soon)

## Learning Objectives

By the end of this module, you will be able to:
* Understand the open-source AI ecosystem and its key components
* Set up a development environment for LLMs using ROCm and AMD GPUs
* Run and evaluate different open-source LLMs locally
* Deploy LLMs using production-ready serving solutions
* Build a simple chat application using Streamlit

We suggest watching videos in the same order as in this document.

# Introduction
## 1. Introduction to Open-Source AI Ecosystem

* Overview of open-source AI landscape
* Introduction to Large Language Models (LLMs)
* Key players and models in the ecosystem
* Understanding model architectures and capabilities

## 2. Getting Started with Hugging Face

* Introduction to Hugging Face ecosystem
* Model Hub exploration
* Popular open-source LLMs
* Using the Transformers library

# Environment Setup

## 1. ROCm and AMD GPUs

* Introduction to ROCm
* Comparing ROCm vs CUDA
* AMD GPU capabilities for AI/ML
* Setting up ROCm environment

## 2. Saturn Cloud Setup for ROCm + MI300x

* Creating a Saturn Cloud account
* Configuring ROCm environment
* Setting up MI300x GPU instances
* Environment testing and validation

# Hands-on LLM Development

## 1. Running DeepSeek R1 Tutorial

* Model overview and capabilities
* Setting up the environment
* Loading and running the model
* Basic inference and generation

## 2. Building a Streamlit Chat Application

* Creating a basic Streamlit app
* Integrating LLM capabilities
* Building the chat interface
* Handling user interactions

# Serving LLMs with vLLM (Optional)

* Introduction to vLLM
* Setting up the serving environment
* Model deployment best practices
* Performance optimization

# Homework

## Assignment: Running and Serving an Open-Source LLM

The goal of this homework is to get hands-on experience with running and serving different open-source LLMs using Saturn Cloud and ROCm.

### Part 1: Running an Alternative LLM

Choose one of the following open-source LLMs (or propose another one of similar size):
* Phi-2
* Mistral 7B
* Llama2 7B
* Falcon 7B

Tasks:
1. Set up the model on Saturn Cloud with ROCm
2. Run basic inference with the model
3. Document the following metrics:
   * Load time
   * Memory usage
   * Inference time for a standard prompt (we'll provide the prompt)
   * Token generation speed
4. Compare these metrics with DeepSeek R1

### Part 2: Model Serving

Using your chosen model from Part 1:
1. Set up a basic serving endpoint using either:
   * vLLM
   * Text Generation Inference
   * FastAPI
2. Create a simple test client that can:
   * Send prompts to your endpoint
   * Measure response times
   * Handle basic error cases
3. Document your serving setup and performance metrics

# Community Notes

Did you take notes? You can share them here:

* Add your notes here!
