# AI SEO Task Orchestrator

## Overview
**AI SEO Task Orchestrator** is a planning-oriented AI system that acts as the central brain of a future AI-powered SEO team.

The system takes a high-level project or SEO goal and transforms it into a structured execution plan:
- one clear EPIC goal,
- multiple atomic SEO tasks,
- assigned AI agent roles,
- task dependencies and difficulty levels.

AI does **not** execute SEO work — it **orchestrates and coordinates it**.

---

## Core Idea
> **AI as a manager, not a worker.**

This project demonstrates a **multi-agent orchestration pattern**, where:
- one AI agent is responsible for planning,
- execution is delegated to specialized agents (future scope).

---

## Architecture
Manual Trigger
↓
Prompt Input
↓
Normalize Input
↓
AI Orchestrator (Planning Only)
↓
Parse & Validate (Safety Layer)
↓
Task Splitter
↓
Task Registry (Data Table)


---

## Key Components

### AI Orchestrator
Acts as an SEO Team Lead:
- analyzes the goal,
- creates an EPIC,
- decomposes it into tasks,
- assigns tasks to AI agent roles,
- defines dependencies.

### Validation Layer
- parses raw AI output,
- enforces strict JSON schema,
- prevents hallucinated or invalid plans.

### Task Registry
A persistent task database (n8n Data Table):
- each row = one task,
- enables tracking, execution, and scaling,
- serves as system memory.

---

## AI Agent Roles (Logical Model)
- `agent_research`
- `agent_competitor`
- `agent_content_plan`
- `agent_writer`
- `agent_onpage`
- `agent_internal_links`
- `agent_qa`

Agents are planned but **not executed** in this version.

---

## What This Project Demonstrates
- AI system design thinking
- multi-agent orchestration architecture
- separation of planning and execution
- safe AI output handling
- scalable automation foundations

---

## Project Status
**MVP / Architecture Prototype**

Focused on orchestration, not execution.

---

## Author
Built as a portfolio project demonstrating  
**AI orchestration and multi-agent system design**.
