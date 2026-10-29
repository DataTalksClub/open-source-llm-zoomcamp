<h1 align="center">
    <strong>Production AI Agents for Generative Media</strong>
</h1>

<p align="center">
Build, scale and monitor agents that run image, video and audio models on serverless GPUs.<br>
Free · open-source (MIT) · project-based · by Nebius × DataTalks.Club
</p>

<p align="center">
<b>Starts Mon 16 Nov 2026 · Apply by Sun 29 Nov 2026 · <a href="https://courses.datatalks.club/register/production-ai-agents-generative-media/">Apply here</a></b>
</p>

> How do you build a production AI system when an agent can launch expensive, slow, failure-prone GPU workloads that produce large media artifacts?

In this course, you build one production system that handles it: a **Personalized Media Factory**. A record (customer, product, user) goes in. An agent writes the copy, generates an image plus a voice or video asset, evaluates the result, regenerates on failure, and scales from 1 to 1,000+ records with a cost line per asset.

Two datasets ship with the course:

* **Santa gift cards:** personalized gift cards generated for a list of children
* **Product catalog:** ad creative generated for a non-seasonal product catalog

**Format:** 4 modules over 5 weeks (Module 1 runs for two weeks), ~8–10 h/week, plus a capstone project.

1. Make it work
2. Make it intelligent
3. Make it scale
4. Make it production-ready

## What You'll Learn

* How to run image, video and audio models as Jobs and Endpoints on serverless GPUs, without managing a cluster
* How to give agents GPU models as tools (MCP) and build generate → evaluate → regenerate loops
* How to fan out batch workloads on spot instances, handle failures and report cost per asset
* How to add evals, tracing and SLOs so you can say what a media agent costs and when it is good enough to ship

## Modules

### [Module 1: Generative Media Workloads](/01-generative-media-workloads)

Get media generation running reliably on serverless GPUs, from a local script to a containerized GPU worker.

* Landscape: modalities, model families, size/VRAM/latency/quality trade-offs, why video is expensive, licences
* First GPU generation: local script → container → GPU Job → Object Storage
* Containers for generative AI: CUDA/PyTorch images, weights vs image, HF cache, pinned revisions, secrets, I/O
* GPU engineering lab: precision, quantization, attention backends, offloading, VAE tiling, batching, torch.compile, caching, GPU selection, OOM debugging
* Jobs vs Endpoints
* **Homework 1: GPU Media Worker** (image + audio or video, measured on 7 metrics)

### [Module 2: Agents That Use GPUs](/02-agents-that-use-gpus)

Build an agent that plans the work, calls GPU models as tools and handles long-running jobs.

* The agent loop, no framework
* Tools and structured outputs: schemas, validation, retries, idempotency, timeouts, errors, state; tools as an MCP server
* CPU agents + GPU tools: control plane vs compute/data plane
* Long-running tools: async, polling vs events, callbacks, job IDs, state persistence, resume, duplicate execution, job lifecycle
* Agent vs workflow; hybrid architectures
* **Homework 2: Media Agent** (coffee ad: plan → generate → inspect → regenerate → video → narration → voice → assemble → trace)

### [Module 3: Scaling, Reliability and Cost](/03-scaling-reliability-cost)

Go from one request to 1,000, survive failures and know the cost of every asset.

* One request to 1,000: concurrency, queues, backpressure, rate limiting, autoscaling, scale-to-zero, batch vs real-time, jobs vs endpoints, GPU capacity, heterogeneous pools; manifest → Jobs fan-out → fan-in
* Failure engineering: break 11 things, then add retry / timeout / fallback / checkpoint / resume / idempotency / dead-letter; prove kill → resume works
* Cost engineering: cost-per-request model, cost-aware agent (cheap draft → evaluate → expensive)
* Performance optimization: quality/latency/cost frontier, benchmark sweeps
* **Homework 3: Santa Scale Challenge – Media Edition** (100 → 1,000 children, leaderboard)

### [Module 4: Evaluation, Observability and Production](/04-evaluation-observability-production)

Measure quality, trace every run and decide when the system is ready to ship.

* Evaluating generative systems: system / agent / media layers; judges, deterministic checks, human eval; golden set + regression gate
* Observability: one trace that answers "why $1.83 / why 94 s"; traces + metrics + logs, dashboards
* Production architecture: auth, secrets, quotas, abuse, prompt injection, content safety, isolation, retention, licensing, provenance, reproducibility, release (versioning, canary, rollback)
* **Homework 4: SLO on the Homework 3 run** (evals, trace, dashboard, alert, go/no-go)

### [Capstone Project](/projects)

A production multimodal agent that uses at least 2 GPU media models, peer-reviewed. You start it in Module 1 and submit it by **Fri 15 Jan 2027**. Share it publicly and run it on Nebius Serverless AI.

## Who Should Join

* AI/ML engineers adding image, video or audio generation to real systems
* MLOps and platform engineers who own the batch pipeline, scheduling and cost
* Founders and small teams paying for per-call media APIs who want to know when self-hosting wins

**Level:** intermediate to advanced.

## Prerequisites

* Python
* Docker basics
* HTTP APIs
* Command line

No diffusion theory required. Prior LLM or MLOps course experience helps but isn't required.

## Dates

| Event | Date |
|---|---|
| Welcome session | Tue 10 Nov 2026 |
| Module 1 (two weeks) | Mon 16 – Sun 29 Nov 2026 |
| Module 2 | Mon 30 Nov – Sun 6 Dec 2026 |
| Module 3 | Mon 7 – Sun 13 Dec 2026 |
| Module 4 | Mon 14 – Sun 20 Dec 2026 |
| Capstone due | Fri 15 Jan 2027 |

## How to Join

The course is free. Seats on the full track are limited, so it is application-only.

1. [Apply here](https://courses.datatalks.club/register/production-ai-agents-generative-media/) and tell us what you are building.
2. We review every application, usually within 2 business days.
3. Approved applicants get the full track: homework, capstone, peer review and [Nebius Builders Program](https://dev.nebius.com/builders) credits.

Not applying? All materials are in this repo and anyone can follow along. You'll need your own GPU access to run the code.

## Cost

The course itself is free. The workloads run on GPUs, which cost money:

* **Approved applicants:** Nebius Builders Program credits cover the course workloads.
* **Following on your own:** you pay for your own GPU usage. Each module reports cost per asset, so you'll know what a run costs before you scale it.

## Open and Portable

* **License:** MIT
* **Portable code:** works with OpenAI-compatible APIs and any S3-compatible object storage
* **Reference execution layer:** Nebius Serverless AI (Jobs, Endpoints) and Nebius Token Factory

## Your Instructors

* Nebius DevRel team (course content and delivery)
* [Alexey Grigorev](https://linkedin.com/in/agrigorev) (DataTalksClub - course logistics and community)

## About DataTalks.Club

DataTalks.Club is a community of data enthusiasts who learn and grow together. We share knowledge, help each other, and make data science more accessible.

Join us:
• [Website](https://datatalks.club/)
• [Slack Community](https://datatalks.club/slack.html)
• [Newsletter](https://us19.campaign-archive.com/home/?u=0d7822ab98152f5afc118c176&id=97178021aa)
• [Events](http://lu.ma/dtc-events)
• [Calendar](https://calendar.google.com/calendar/?cid=ZjhxaWRqbnEwamhzY3A4ODA5azFlZ2hzNjBAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)
• [YouTube](https://www.youtube.com/@DataTalksClub/featured)
• [GitHub](https://github.com/DataTalksClub)
• [LinkedIn](https://www.linkedin.com/company/datatalks-club/)
• [Twitter](https://twitter.com/DataTalksClub)
