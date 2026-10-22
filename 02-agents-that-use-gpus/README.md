# Module 2: Agents That Use GPUs

Welcome to Module 2 of Production AI Agents for Generative Media! This week we make it intelligent: give agents GPU models as tools and build generate → evaluate → regenerate loops.

* Video Link (Coming Soon)
* Slides (Coming Soon)

## Learning Objectives

By the end of this module, you will be able to:

* Implement the agent loop from scratch, no framework
* Design tools with schemas, validation, retries, idempotency, timeouts and error handling; expose tools as an MCP server
* Separate the CPU control plane from the GPU compute/data plane
* Handle long-running tools: async execution, polling vs events, callbacks, job IDs, state persistence, resume, duplicate execution, job lifecycle
* Choose between agent, workflow and hybrid architectures for a media task

## 2.0 The Agent Loop, No Framework

* Plan → act → observe, written out explicitly
* Where state lives and what survives a restart

## 2.1 Tools and Structured Outputs

* Schemas, validation, retries
* Idempotency, timeouts, errors, state
* Tools as an MCP server

## 2.2 CPU Agents + GPU Tools

* Control plane vs compute/data plane
* Why the agent itself never needs a GPU

## 2.3 Long-Running Tools

* Async execution, polling vs events, callbacks
* Job IDs, state persistence, resume
* Duplicate execution and the job lifecycle

## 2.4 Agent vs Workflow

* When a fixed pipeline wins, when an agent wins
* Hybrid architectures for media generation

## Homework 2: Media Agent

Build a media agent for a coffee ad: plan → generate → inspect → regenerate → video → narration → voice → assemble, with a full trace of every step.

The agent must evaluate intermediate assets and regenerate on failure instead of accepting the first output.

# Community Notes

Did you take notes? You can share them here:

* Add your notes here!
