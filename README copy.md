<p align="center">
  [to do] <img width="100%" src="images/architecture/llm_zoomcamp_overview.jpg" alt="Open-Source LLM Zoomcamp Overview">
</p>

<h1 align="center">
    <strong>Open-Source LLM Zoomcamp: Building and Deploying LLMs on AMD Hardware</strong>
</h1>

<p align="center">
Master the fundamentals of building, fine-tuning, and deploying open-source large language models (LLMs) on high-performance AMD hardware. Gain hands-on experience with ROCm-enabled MI300x GPUs hosted on Saturn Cloud.
</p>

<p align="center">
[to do] <a href="https://airtable.com/shr6oVXeQvSI5HuWD"><img src="https://user-images.githubusercontent.com/875246/185755203-17945fd1-6b64-46f2-8377-1011dcb1a444.png" height="50" /></a>
</p>

<p align="center">
<a href="https://datatalks.club/slack.html">Join Slack</a> •
<a href="https://app.slack.com/client/T01ATQK62F8/C01FABYF2RG">#course-llm Channel</a> •
<a href="https://t.me/llmzoomcamp">Telegram Announcements</a> •
<a href="https://www.youtube.com/playlist?list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb">Course Playlist</a> •
<a href="https://docs.google.com/document/d/19bnYs80DwuUimHM65UV3sylsCn2j1vziPOwzBwQrebw/edit?usp=sharing">FAQ</a>
</p>

## Course Goal

Equip participants with the practical skills required to **build, fine-tune, and deploy open-source large-language-model (LLM) systems** on high-performance AMD hardware—specifically ROCm-enabled MI300x GPUs hosted on Saturn Cloud.

## Target Audience

| Level | Profile | Typical Motivation |
| --- | --- | --- |
| **Intermediate → Advanced ML / AI practitioners** | Already train or deploy models; want to master open-source LLM stacks | Replace / complement proprietary SaaS solutions |
| **Software engineers pivoting to AI** | Strong engineering background; limited LLM experience | Fast, hands-on on-ramp to production LLMs |
| **Researchers & OSS contributors** | Academic or open-source focus | Gain reproducible, industry-grade deployment skills |
| **Infra / MLOps teams exploring AMD** | Evaluate ROCm vs. CUDA cost-performance | Build internal reference architectures |

## Format & Logistics

| Item | Details |
| --- | --- |
| **Modules** | 2 core modules (additional bonus labs possible) |
| **Micro-lectures** | 7–15 videos per module (5–15 min each) → **60–90 min total per module** |
| **Labs & Notebooks** | Hosted on Saturn Cloud with MI300x GPUs; zero local setup |
| **Homework** | Auto-graded forms; ensures hands-on interaction with ROCm stack |
| **Capstone Project** | Peer-reviewed; mandatory for certificate |
| **Certificate** | Issued upon: ① all homeworks passed + ② capstone accepted |

## How to Enroll

### 2025 Cohort
- **Start Date**: May 14, 2025
- **Register Here**: [Sign up](https://airtable.com/shr6oVXeQvSI5HuWD)
- **Access Cohort Materials**: [2025 Cohort Folder](cohorts/2025/)

### Self-Paced Learning
All course materials are freely available for independent study. Follow these steps:
1. Watch the course videos
2. Join the [Slack community](https://datatalks.club/slack.html)
3. Refer to the [FAQ document](https://docs.google.com/document/d/19bnYs80DwuUimHM65UV3sylsCn2j1vziPOwzBwQrebw/edit?usp=sharing) for guidance

## Prerequisites
To get the most out of this course, you should have:
- Python programming experience
- Basic understanding of machine learning concepts
- Familiarity with deep learning frameworks (PyTorch preferred)
- No prior LLM experience required

## Module Breakdown

### Module 1: Running & Deploying Open-Source LLMs
- Course orientation
- OSS-AI ecosystem overview
- LLM foundations & model zoo (Hugging Face)
- ROCm vs. CUDA: concepts & migration tips
- Saturn Cloud quick-start (ROCm + MI300x image)
- Tutorial: run DeepSeek-Coder-R1
- Build a minimal Streamlit chat UI
- Serving options (vLLM, TGI, Ollama)
- Homework

### Module 2: Fine-Tuning & Domain Adaptation
- PEFT vs. full fine-tuning trade-offs
- Llama-Factory workflow
- Dataset curation & cleaning
- Tutorial: fine-tune DeepSeek-Coder-R1
- Upgrade the Streamlit chatbot with new weights
- Bonus lab: ROCm-accelerated text-to-image
- Homework & Capstone Project

## Assessment & Certification

| Requirement | Weight |
| --- | --- |
| All auto-graded homeworks | Pass / fail |
| Capstone project | 100 pts |
| **≥ 70 pts → Certificate** | Signed by AMD × Saturn Cloud |

Top-scoring projects will be showcased on the course repo and AMD developer hub.

## AMD-Specific Resources
- "Building LLMs with ROCm" primer
- Example notebooks: LLM inference, text-to-image diffusion, MI300x performance tuning
- Dedicated MI300x instances reserved for cohorts

## References & Starter Code
- [DataTalksClub/llm-zoomcamp](https://github.com/DataTalksClub/llm-zoomcamp)
- Saturn Cloud public templates for ROCm + MI300x
- Hugging Face "Open LLM Leaderboard"

## Community & Support

### Getting Help on Slack
Join the [`#course-llm`](https://app.slack.com/client/T01ATQK62F8/C01FABYF2RG) channel on [DataTalks.Club Slack](https://datatalks.club/slack.html) for discussions, troubleshooting, and networking.

To keep discussions organized:
- Follow [our guidelines](asking-questions.md) when posting questions
- Review the [community guidelines](https://datatalks.club/slack/guidelines.html)

## Meet the Instructors
- [Alexey Grigorev](https://linkedin.com/in/agrigorev)
- [AMD Developer Relations Team](https://www.amd.com)
- [Saturn Cloud Team](https://saturncloud.io)

## About DataTalks.Club

<p align="center">
  <img width="40%" src="https://github.com/user-attachments/assets/1243a44a-84c8-458d-9439-aaf6f3a32d89" alt="DataTalks.Club">
</p>

<p align="center">
<a href="https://datatalks.club/">DataTalks.Club</a> is a global online community of data enthusiasts. It's a place to discuss data, learn, share knowledge, ask and answer questions, and support each other.
</p>

<p align="center">
<a href="https://datatalks.club/">Website</a> •
<a href="https://datatalks.club/slack.html">Join Slack Community</a> •
<a href="https://us19.campaign-archive.com/home/?u=0d7822ab98152f5afc118c176&id=97178021aa">Newsletter</a> •
<a href="http://lu.ma/dtc-events">Upcoming Events</a> •
<a href="https://calendar.google.com/calendar/?cid=ZjhxaWRqbnEwamhzY3A4ODA5azFlZ2hzNjBAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ">Google Calendar</a> •
<a href="https://www.youtube.com/@DataTalksClub/featured">YouTube</a> •
<a href="https://github.com/DataTalksClub">GitHub</a> •
<a href="https://www.linkedin.com/company/datatalks-club/">LinkedIn</a> •
<a href="https://twitter.com/DataTalksClub">Twitter</a>
</p>

*Version 2025-05-14 — ready for internal review*

