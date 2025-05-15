# Module 1: Introduction to Open-Source AI and LLMs

<div align="center">
  <img src="https://raw.githubusercontent.com/kavaivaleri/open-source-llm-zoomcamp/main/images/module-1-cover.png" alt="Module 1 Cover - Introduction to Open-Source AI and LLMs" width="800">
</div>

Welcome to Module 1 of the Open Source LLM Zoomcamp! In this module, we'll explore how to run and deploy these powerful models using AMD GPUs and modern cloud infrastructure.

* Video Link (Coming Soon)
* Slides (Coming Soon)

## Table of Contents
- [Learning Objectives](#learning-objectives)
- [1. Introduction](#1-introduction)
  - [1.1 Introduction to Open-Source AI Ecosystem](#11-introduction-to-open-source-ai-ecosystem)
  - [1.2 Getting Started with Hugging Face](#12-getting-started-with-hugging-face)
- [2. Environment Setup](#2-environment-setup)
  - [2.1 ROCm and AMD GPUs](#21-rocm-and-amd-gpus)
  - [2.2 Saturn Cloud Setup for ROCm + MI300x](#22-saturn-cloud-setup-for-rocm--mi300x)
- [3. Hands-on LLM Development](#3-hands-on-llm-development)
  - [3.1 Running DeepSeek R1 Tutorial](#31-running-deepseek-r1-tutorial)
  - [3.2 Building a Streamlit Chat Application](#32-building-a-streamlit-chat-application)
- [4. Serving LLMs with vLLM (Optional)](#4-serving-llms-with-vllm-optional)
- [5. Homework: Running and Serving an Open-Source LLM](#5-homework-running-and-serving-an-open-source-llm)
- [Community Notes](#community-notes)

## Learning Objectives

By the end of this module, you will be able to:
* Understand the open-source AI ecosystem and its key components
* Set up a development environment for LLMs using ROCm and AMD GPUs
* Run and evaluate different open-source LLMs locally
* Deploy LLMs using production-ready serving solutions
* Build a simple chat application using Streamlit

We recommend watching the videos in the order presented in this document.
# 1. Introduction
## 1.1 Introduction to Open-Source AI Ecosystem

* Overview of open-source AI landscape
* Introduction to Large Language Models (LLMs)
* Key players and models in the ecosystem
* Understanding model architectures and capabilities

## 1.2 Getting Started with Hugging Face

* Introduction to Hugging Face ecosystem
* Model Hub exploration
* Popular open-source LLMs
* Using the Transformers library

# 2. Environment Setup

## 2.1 ROCm and AMD GPUs

* Introduction to ROCm
* Comparing ROCm vs CUDA
* AMD GPU capabilities for AI/ML
* Setting up ROCm environment

## 2.2 Saturn Cloud Setup for ROCm + MI300x

* Creating a Saturn Cloud account
* Configuring ROCm environment
* Setting up MI300x GPU instances
* Environment testing and validation

# 3. Hands-on LLM Development

## 3.1 Running DeepSeek R1 Tutorial

* Model overview and capabilities
* Setting up the environment
* Loading and running the model
* Basic inference and generation

## 3.2 Building a Streamlit Chat Application

* Creating a basic Streamlit app
* Integrating LLM capabilities
* Building the chat interface
* Handling user interactions

# 4. Serving LLMs with vLLM (Optional)

* Introduction to vLLM
* Setting up the serving environment
* Model deployment best practices
* Performance optimization

# 5. Homework: Running and Serving an Open-Source LLM

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
