# Module 1: Generative Media Workloads

Welcome to Module 1 of Production AI Agents for Generative Media! This week we make it work: run image, video and audio models on serverless GPUs and build a reliable GPU media worker.

* Video Link (Coming Soon)
* Slides (Coming Soon)

## Learning Objectives

By the end of this module, you will be able to:

* Compare generative media modalities and model families (size, VRAM, latency, quality trade-offs) and explain why video is expensive
* Run your first GPU generation: local script → container → GPU Job → Object Storage
* Write a production Dockerfile for generative AI (CUDA/PyTorch images, weights vs image, HF cache, pinned revisions, secrets, I/O)
* Apply GPU engineering techniques: precision, quantization, attention backends, offloading, VAE tiling, batching, `torch.compile`, caching, GPU selection, OOM debugging
* Choose between Jobs and Endpoints for a media workload

## 1.1 Landscape: Modalities and Model Families

* Modalities: image, video, audio — what changes between them
* Model families (high level): size, VRAM, latency, quality
* Why video is expensive
* Licences: what you can and cannot ship

## 1.2 First GPU Generation

* Local script → container → GPU Job → Object Storage
* Reference execution layer: Nebius Serverless AI (Jobs, Endpoints) and Nebius Token Factory
* Code is OpenAI- and S3-compatible, so the pattern ports elsewhere

## 1.3 Containers for Generative AI

* CUDA/PyTorch base images
* Weights vs image: what goes where, HF cache, pinned revisions
* Secrets and I/O handling
* Bad Dockerfile → production Dockerfile

## 1.4 GPU Engineering Lab

* Precision and quantization
* Attention backends
* Offloading, VAE tiling, batching
* `torch.compile`, caching
* GPU selection and OOM debugging

## 1.5 Jobs vs Endpoints

* When a Job is the right primitive, when an Endpoint is
* What this choice implies for cost, latency and scaling (preview of Module 3)

## Homework 1: GPU Media Worker

Build a GPU media worker that generates an image plus an audio or video asset.

Report 7 metrics for your run (e.g. latency, GPU time, VRAM used, cost estimate, output size, retries/failures, quality notes). Store outputs in Object Storage with pinned model revisions so the run is reproducible.

# Community Notes

Did you take notes? You can share them here:

* Add your notes here!
