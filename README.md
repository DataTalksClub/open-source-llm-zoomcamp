<h1 align="center">
    <strong>Production AI Agents for Generative Media</strong>
</h1>

<p align="center">
Build, scale and monitor agents that run GPU image, video and audio models on Nebius Serverless AI. Free, open-source (MIT), project-based.
</p>

> How do you build a production AI system when an agent can launch expensive, slow, failure-prone GPU workloads that produce large media artifacts?

In this course you build one production system that handles it: a **Personalized Media Factory**. A record (customer, product, user) goes in. An agent writes the copy, generates an image plus a voice or video asset, evaluates the result, regenerates on failure, and scales from 1 to 1,000+ records with a cost line per asset.

Two datasets ship with the course: a **Santa gift-card run** and a **non-seasonal product catalog to ad creative run**.

* 4 modules over 5 weeks (Module 1 is two weeks) · ~8-10 h/week · free · open-source · project-based
* Week 1: Make it work
* Week 2: Make it intelligent
* Week 3: Make it scale
* Week 4: Make it production-ready

## What You'll Learn

* How to run image, video and audio models as Jobs and Endpoints on serverless GPUs, without managing a cluster
* How to give agents GPU models as tools (MCP) and build generate, evaluate, regenerate loops
* How to fan out batch workloads on spot instances, handle failures and report cost per asset
* How to add evals, tracing and SLOs so you can say what a media agent costs and when it is good enough to ship

## Modules

### [Module 1: Generative Media Workloads](/01-generative-media-workloads)

Build consistent media generation on serverless GPUs.

* Landscape: modalities, model families, size/VRAM/latency/quality, why video is expensive, licences
* First GPU generation: local script → container → GPU Job → Object Storage
* Containers for generative AI: CUDA/PyTorch images, weights vs image, HF cache, pinned revisions, secrets, I/O
* GPU engineering lab: precision, quantization, attention backends, offloading, VAE tiling, batching, torch.compile, caching, GPU selection, OOM debugging
* Jobs vs Endpoints
* Homework 1: GPU Media Worker (image + audio or video, 7 metrics)

### [Module 2: Agents That Use GPUs](/02-agents-that-use-gpus)

Orchestrate multi-agent media generation workflows.

* The agent loop, no framework
* Tools and structured outputs: schemas, validation, retries, idempotency, timeouts, errors, state; tools as an MCP server
* CPU agents + GPU tools: control plane vs compute/data plane
* Long-running tools: async, polling vs events, callbacks, job IDs, state persistence, resume, duplicate execution, job lifecycle
* Agent vs workflow; hybrid architectures
* Homework 2: Media Agent (coffee ad: plan → generate → inspect → regenerate → video → narration → voice → assemble → trace)

### [Module 3: Scaling, Reliability and Cost](/03-scaling-reliability-cost)

Scale batch media generation.

* One request to 1,000: concurrency, queues, backpressure, rate limiting, autoscaling, scale-to-zero, batch vs real-time, jobs vs endpoints, GPU capacity, heterogeneous pools; manifest → Jobs fan-out → fan-in
* Failure engineering: break 11 things, then retry / timeout / fallback / checkpoint / resume / idempotency / dead-letter; kill → resume proof
* Cost engineering: cost-per-request model, cost-aware agent (cheap draft → evaluate → expensive)
* Performance optimization: quality/latency/cost frontier, benchmark sweeps
* Homework 3: Santa Scale Challenge - Media Edition (100 → 1,000 children, leaderboard)

### [Module 4: Evaluation, Observability and Production](/04-evaluation-observability-production)

Evaluate, trace and set SLOs for media generation agents.

* Evaluating generative systems: system / agent / media layers; judges, deterministic checks, human eval; golden set + regression gate
* Observability: one trace, "why $1.83 / why 94 s"; traces + metrics + logs, dashboards
* Production architecture: auth, secrets, quotas, abuse, prompt injection, content safety, isolation, retention, licensing, provenance, reproducibility, release (versioning, canary, rollback)
* Homework 4: SLO on the Homework 3 run (evals, trace, dashboard, alert, go/no-go)

### [Capstone Project](/projects)

A production multimodal agent that uses at least 2 GPU media models, peer-reviewed. It starts in Module 1 and is due **15 Jan 2027**. Share it publicly and run it on Nebius Serverless AI.

## Who Should Join

* AI/ML engineers adding image, video or audio generation to real systems
* MLOps and platform engineers who own the batch pipeline, scheduling and cost
* Founders and small teams paying per-call media APIs who want to know when self-hosting wins

Medium-advanced level. Application only, limited seats - tell us what you are building.

## Prerequisites

Python, Docker basics, HTTP APIs, command line. No diffusion theory required. Prior LLM or MLOps course experience helps, not required.

## Open and Portable

MIT license. Code is OpenAI- and S3-compatible. Nebius Serverless AI (Jobs, Endpoints) and Nebius Token Factory are the reference execution layer.

## How to Join

Application only, limited seats. Tell us what you are building. We review every application, usually within 2 business days. Approved applicants get the full path (homework, capstone, peer review) and Nebius Builders Program credits. Everyone can follow the public repo.

## Dates

* Welcome session: Tue 10 Nov 2026
* Course starts: Mon 17 Nov 2026 · apply by Wed 26 Nov 2026
* Module 1 (two weeks): 17-30 Nov 2026 (through Sun 30 Nov)
* Module 2: 1-7 Dec 2026
* Module 3: 8-14 Dec 2026
* Module 4: 15-21 Dec 2026
* Course ends: Sun 21 Dec 2026
* Capstone due: Fri 15 Jan 2027

## Your Instructors

* Nebius DevRel team (course content and delivery)
* [Alexey Grigorev](https://linkedin.com/in/agrigorev) (DataTalksClub - course logistics and community)

## About DataTalks.Club

DataTalks.Club is a community of data enthusiasts learning and growing together. We're all about sharing knowledge, helping each other out, and making data science more accessible.

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
