# Distributed Decision-Making Agents using AutoGen AG2, Ollama and Serper Search

## Overview

This project demonstrates a multi-agent decision-making system built using AutoGen AG2, Ollama, and Google Serper Search.

The system simulates a collaborative research team where multiple AI agents independently investigate different perspectives of a problem and provide evidence to a decision-making agent. The final agent evaluates the collected information and generates a recommendation based on the available evidence.

The project explores one of the most important patterns in Agentic AI systems:

Research Agents → Evidence Collection → Judge Agent → Final Decision

This architecture is commonly used in autonomous research systems, planning agents, evaluation pipelines, and enterprise AI workflows.

---

## Project Objective

The primary goal of this project is to understand how multiple AI agents can:

* Work independently on specialized tasks
* Gather and analyze information
* Collaborate through structured workflows
* Produce evidence-based decisions
* Utilize external tools to improve reasoning quality

---

## Technologies Used

### Framework

* AutoGen AG2 (v0.9.7)

### Large Language Model

* Qwen2.5:7B
* Ollama

### Search Engine

* Google Serper API

### Development Environment

* Python 3.9
* Jupyter Notebook

---

## Architecture

### High-Level Workflow

```text
                   User Query
                        │
                        ▼
            ┌────────────────────┐
            │  Research Problem  │
            └────────────────────┘
                        │
            ┌───────────┴───────────┐
            │                       │
            ▼                       ▼
   Pros Research Agent      Cons Research Agent
            │                       │
            ▼                       ▼
     Web Search Tool         Web Search Tool
            │                       │
            ▼                       ▼
      Evidence Report       Evidence Report
            └───────────┬───────────┘
                        ▼
                 Judge Agent
                        │
                        ▼
                Final Decision
```

---

## Agent Responsibilities

### Pros Research Agent

Responsibilities:

* Search for positive aspects
* Collect supporting evidence
* Summarize key benefits
* Present arguments in favor

Example:

```text
Advantages of AutoGen
Benefits of Agent Frameworks
Positive Use Cases
```

---

### Cons Research Agent

Responsibilities:

* Search for limitations
* Identify risks and drawbacks
* Summarize challenges
* Present arguments against adoption

Example:

```text
Framework Limitations
Scalability Challenges
Complexity Considerations
```

---

### Judge Agent

Responsibilities:

* Evaluate both perspectives
* Compare evidence
* Generate final recommendation
* Provide supporting rationale

Example Output:

```text
Decision: Adopt

Reason:
Benefits outweigh the identified limitations.
```

---

## Workflow

### Step 1: Research

Each research agent performs independent investigation.

```text
Research Question
        │
        ▼
 Search Results
        │
        ▼
 Agent Analysis
```

---

### Step 2: Evidence Collection

The agents summarize findings into concise reports.

```text
Search Results
      │
      ▼
Evidence Summary
```

---

### Step 3: Decision Making

The Judge Agent receives both reports.

```text
Pros Report
      +
Cons Report
      │
      ▼
 Judge Agent
      │
      ▼
Final Decision
```

---

## Features

### Multi-Agent Architecture

Multiple specialized agents collaborate to solve a problem.

### Tool-Augmented Research

Agents use external search tools to gather current information.

### Evidence-Based Reasoning

Decisions are based on collected evidence rather than relying solely on model memory.

### Agent Orchestration

Independent agents contribute to a larger decision-making workflow.

### Local LLM Deployment

The system runs using a locally hosted Qwen2.5 model through Ollama.

---

## Repository Structure

```text
.
├── Distributed_Decision_Making_Agents_AG2.ipynb
└── README.md
```

---

## Concepts Demonstrated

This project demonstrates:

* Agentic AI Systems
* Multi-Agent Collaboration
* Agent Orchestration
* Tool Calling
* Web Search Integration
* Decision Aggregation
* Evidence-Based Reasoning
* Autonomous Research Workflows
* Local LLM Integration
* AutoGen AG2 Framework

---

## Learning Outcomes

Through this project the following concepts were implemented and explored:

### Agent Communication

Agents operate independently while contributing to a shared objective.

### Research Agent Pattern

Specialized agents investigate different aspects of a problem.

### Judge Agent Pattern

A decision-making agent evaluates evidence and produces conclusions.

### Tool Integration

External search capabilities enhance agent reasoning quality.

### Multi-Agent Workflows

Complex tasks are decomposed into smaller specialized responsibilities.

---

## Future Enhancements

Potential future improvements include:

* Critic Agent Integration
* Reviewer Agent Pattern
* Fact Verification Agents
* RAG-Based Knowledge Sources
* Memory-Enabled Agents
* Multi-Step Planning Agents
* Autonomous Research Teams
* Real-Time Data Sources
* Web Dashboard Interface

---

## Conclusion

This project demonstrates how autonomous AI agents can collaborate through structured workflows to gather evidence, analyze information, and make informed decisions.

By combining AutoGen AG2, Ollama, and external search tools, the system illustrates a practical implementation of distributed decision-making and multi-agent orchestration patterns commonly used in modern Agentic AI applications.
