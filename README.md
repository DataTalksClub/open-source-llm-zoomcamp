<h1 align="center">
    <strong>Production AI Agents for Generative Media</strong>
</h1>

<p align="center">
Build, scale and monitor agents that run image, video and audio models on serverless GPUs.<br>
Free · open-source (MIT) · project-based · by Nebius × DataTalks.Club
</p>

<p align="center">
<b>Starts Mon 16 Nov 2026 · Apply by Mon 30 Nov 2026 · <a href="https://courses.datatalks.club/register/production-ai-agents-generative-media/">Apply here</a></b>
</p>

> How do you build a production AI system when an agent can launch expensive, slow, failure-prone GPU workloads that produce large media artifacts?

Media agents are an engineering problem, not a prompting problem. In this course, you build one production system that handles it: a **Personalized Media Factory**.

1. **Input:** a brief, made of a task prompt, a data record and constraints (format, style, budget)
2. **Agent (LLM):** plans the asset and writes its text, such as a card message or an ad script
3. **GPU models:** generate an image plus voice or video
4. **Check:** regenerates the asset when it is not good enough
5. **Scale:** from 1 to 1,000+ records, with a cost per asset

Two examples run through the course:

* **Santa Christmas Challenge (worked example):** a child profile becomes a personalized gift card with a Santa voice message
* **Product catalog (capstone example):** a product record becomes ad creative with a voice-over or a short video. When it fails the check, the agent revises and regenerates

**Format:** a Welcome session (Module 0), then 4 modules over 5 weeks (Module 1 runs for two weeks), ~8–10 h/week, plus a capstone project. Lectures are pre-recorded, with a weekly live office hour.

1. Make it work
2. Make it intelligent
3. Make it scale
4. Make it production-ready

## What You'll Learn

* How to run image, video and audio models as Jobs and Endpoints on serverless GPUs, without managing a cluster
* How to give agents GPU models as tools (MCP) and build generate → evaluate → regenerate loops
* How to fan out batch workloads on spot GPUs, handle failures and report cost per asset
* How to add evals, tracing and SLOs so you can say what a media agent costs and when it is good enough to ship

## Modules

### Module 0: Welcome

Tue 10 Nov 2026, live. Why media agents are an engineering problem, not a prompting problem.

* The factory end to end
* Real projects from Nebius customers and partners
* **You leave with:** your starting point and setup

### [Module 1: Consistent Media Generation on Serverless GPUs](/01-generative-media-workloads)

Mon 16 – Sun 29 Nov 2026 (two weeks)

* Media model landscape
* Templates, containers and model cache
* Seeds
* Fitting VRAM
* Measuring startup, load and generation time
* **Homework 1: GPU Media Worker** (a spec in, an asset plus a cost breakdown out)
* **Capstone proposal**

### [Module 2: Multi-Agent Media Workflows](/02-agents-that-use-gpus)

Mon 30 Nov – Sun 6 Dec 2026

* The agent loop from scratch
* GPU models as typed tools over MCP
* Long-running tools
* Planner / generator / reviewer
* **Homework 2: Media Agent** (a 10-second ad plus an execution trace), due Sun 6 Dec

### [Module 3: Batch Media Generation at Scale](/03-scaling-reliability-cost)

Mon 7 – Sun 13 Dec 2026

* Fan-out on spot GPUs
* Per-item checkpoints
* Breaking the pipeline on purpose
* Budget-aware agents
* Quality vs cost
* **Homework 3: Factory Scale Challenge** (1,000 records, public leaderboard), due Sun 13 Dec

### [Module 4: Evals, Tracing and SLOs](/04-evaluation-observability-production)

Mon 14 – Sun 20 Dec 2026

* System, agent and media evals
* Multimodal judges
* Cost and time per step
* SLO, dashboard and alert
* No homework: you apply Module 4 in your capstone (**capstone brief**)

### [Capstone Project](/projects)

A multimodal agent using at least two GPU media models, shared publicly and running on Nebius Serverless AI. You write the proposal in Module 1 and submit the project by **Fri 15 Jan 2027**, then review your peers' projects.

Your project needs:

* An agent with 2+ tools
* An async GPU workload
* Assets in object storage
* An eval suite
* Tracing
* An SLO
* A cost report
* Proof that a killed run resumes without redoing finished work

Ideas: a marketing studio, podcast producer, video localization, storybook generator, product ad agent or paper-to-explainer video.

## Who Should Join

Working builders running open or custom GPU media models:

* AI/ML engineers adding image, video or audio generation to real systems
* MLOps and ML platform engineers who own the batch pipeline, scheduling and cost line
* Technical founders and small teams paying for per-call media APIs who need to know when self-hosting wins

**Level:** intermediate to advanced.

## Prerequisites

* Python
* Docker basics
* HTTP APIs
* Command line

Prior LLM or MLOps course experience helps but isn't required.

**Not covered:** diffusion maths, training foundation models, deep fine-tuning, CUDA, Kubernetes, RAG, LLM fundamentals.

## Dates

All times are CET (Berlin). Modules run Monday to Sunday.

| Date | What | Due / live session |
|---|---|---|
| Tue 3 Nov 2026 | Promo workshop: "Build a Media Agent: CPU Agent, GPU Models as Tools" | Live, 16:30–18:00 · [Register](https://luma.com/tj2nbrl2) |
| Tue 10 Nov 2026 | Module 0: Welcome session and pre-course Q&A | Live, 17:00–18:00 · [Register](https://luma.com/i4x6x2zy) |
| Mon 16 Nov 2026 | Course launch | Live, 17:00–18:00 · [Register](https://luma.com/xey7h50c) |
| Mon 16 – Sun 29 Nov 2026 | Module 1 (two weeks) | Homework 1 and capstone proposal |
| Mon 30 Nov – Sun 6 Dec 2026 | Module 2 | Homework 2, due Sun 6 Dec |
| Mon 30 Nov 2026 | Applications close | |
| Mon 7 – Sun 13 Dec 2026 | Module 3 | Homework 3 (leaderboard), due Sun 13 Dec |
| Mon 14 – Sun 20 Dec 2026 | Module 4 | Capstone brief |
| Fri 15 Jan 2027 | Capstone due, then peer review | Capstone |

Materials and dates may change.

## How to Join

The course is free. Seats in the live cohort are limited, so it is application only.

1. [Apply here](https://courses.datatalks.club/register/production-ai-agents-generative-media/) and tell us what you are building.
2. We review every application, usually within 2 business days.
3. Approved applicants join the live cohort: shared deadlines, peer-reviewed homework and the capstone.
4. Get GPU credits through the [Nebius AI Builder Program](https://dev.nebius.com/builders).

"Live cohort" means shared deadlines and peer-reviewed homework, not mandatory live classes. Lectures are pre-recorded, and there is a weekly live office hour.

Not applying? All materials are in this repo and anyone can follow along. You'll need your own GPU access to run the code.

## Cost

The course itself is free. The workloads run on GPUs, which cost money:

* **GPU credits:** applicants get credits through the [Nebius AI Builder Program](https://dev.nebius.com/builders), which is free to join. Usage beyond the credits is billed to your account.
* **Following on your own:** you pay for your own GPU usage.

Each module reports cost per asset, so you'll know what a run costs before you scale it.

## What You Will Use

| Layer | Course default | Alternatives |
|---|---|---|
| Media runtimes | Hugging Face Diffusers, model-specific runtimes | ComfyUI for prototyping |
| Models | Image: Qwen-Image / FLUX-class, Sana · Video: Wan · Audio: Kokoro / Chatterbox TTS, Whisper | Any open-weights equivalent |
| LLM | Nebius Token Factory (OpenAI-compatible) | Self-hosted vLLM, any OpenAI-compatible API |
| Agents and tools | Raw tool calling → MCP | Pydantic AI, LangGraph |
| GPU compute | Nebius Serverless AI: Jobs, Endpoints | DevLabs with JupyterLab |
| Storage and API | S3-compatible Object Storage · FastAPI | Gradio, Streamlit |
| Tracking, tracing, evals | To be announced | Langfuse, OpenTelemetry |

## Open and Portable

* **License:** MIT
* **Portable code:** OpenAI- and S3-compatible, so you can run it elsewhere
* **Reference platform:** Nebius Serverless AI (Jobs, Endpoints) and Nebius Token Factory
* **Model licences:** open-weights models come with their own licences. Check before commercial use.

## Your Instructors and Partners

* Nebius DevRel team (course content and delivery)
* [Nebius Academy](https://nebius.com/certification) (content and expert support)
* [Alexey Grigorev](https://linkedin.com/in/agrigorev) (DataTalks.Club: course logistics and community)

Nebius in the course:

* [Nebius Serverless AI](https://nebius.com/serverless): the reference platform for code-alongs and homework. Run containerized AI workloads on GPUs without managing infrastructure.
* [Nebius AI Builder Program](https://dev.nebius.com/builders): how applicants get GPU credits. Free to join: credits, runnable examples and cookbooks, technical office hours and a community of AI builders.

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
