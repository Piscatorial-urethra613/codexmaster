# Codex Master

A structured Codex system combined with a Website Blueprint Generator to produce consistent, non-generic AI-generated websites.

## The Problem

AI-generated websites tend to:
- reuse the same layouts
- ignore design intent
- produce inconsistent results across runs

## The Solution

Codex Master solves this with two systems:

### 1. Execution System (Codex Master)
Enforces structured workflows, validation, and consistency.

### 2. Blueprint Generator
Forces design diversity by generating varied, non-repetitive website structures before execution.

Result:
- consistent builds
- non-generic design
- repeatable outcomes


## Overview

This system turns Codex from a free-form assistant into a structured engineering agent.

Every task is:
- routed
- executed through a defined workflow
- validated for correctness
- measured for quality
- improved through feedback


## System Pipeline

Route → Resolve → Execute → Validate → Measure → Improve → Recover

A closed-loop system that prevents drift, enforces correctness, and continuously improves output quality.

---

Each layer is modular and can be used independently or as part of the full system.

## Core Components

### Governance Layer
Defines rules, priorities, and system boundaries.

- [Guardrails](./docs/security/guardrails.md)
- instruction_priority.md
- model_instructions.md
- [System Contract](./docs/security/system_contract.md)

---

### Input & Context Layer
Determines task classification and relevant context.

- [Task Router](./docs/workflow/task_router.md)
- [Context Resolver](./docs/development/context_resolver.md)
- [State Manager](./docs/workflow/state_manager.md)

---

### Execution Layer
Controls how tasks are performed.

- [Workflow Engine](./docs/workflow/workflow_engine.md)
- [Agent Workflow](./docs/workflow/agent_workflow.md)
- task_template.md
- change_planning.md

---

### Validation Layer
Ensures correctness and completeness.

- [Validation Agent](./docs/workflow/validation_agent.md)
- [Metrics] (./docs/strategy/metrics.md)

---

### Recovery Layer
Handles failures and system resilience.

- [Failure Handler](./docs/security/failure_handler.md)
- [Debugging Playbook](./docs/security/debugging_playbook.md)

---

### Optimization Layer
Improves performance over time.

- [Prompt Optimizer] (./docs/strategy/prompt_optimizer.md)

---

### Engineering Standards
Maintains code quality and consistency.

- [Architecture](./docs/architecture/architecture.md)`
- [Code Style] (./docs/development/code_style.md)
- anti_overengineering.md
- repo_map.md
- environment.md

---

## Key Properties

### Deterministic Execution
Tasks follow structured workflows instead of ad-hoc reasoning.

### Context Awareness
Conflicting inputs are resolved using defined priority rules.

### Reliability
Outputs are validated and measured before acceptance.

### Continuous Improvement
Failures and metrics drive system refinement.

### Scalability
Modular components allow extension without breaking behavior.

---

## Execution Flow

All tasks follow this sequence:

1. **Task Routing**  
   Classify task type and complexity (`[Task Router](./docs/workflow/task_router.md))

2. **Context Resolution**  
   Determine authoritative context (`[Context Resolver](./docs/development/context_resolver.md), `[State Manager](./docs/workflow/state_manager.md))

3. **Execution**  
   Run through enforced workflow (`[Workflow Engine](./docs/workflow/workflow_engine.md))

4. **Validation**  
   Verify correctness (`[Validation Agent](./docs/workflow/validation_agent.md))

5. **Metrics Evaluation**  
   Measure quality (`[Metrics] (./docs/strategy/metrics.md))

6. **Failure Handling (if needed)**  
   Classify and recover (`[Failure Handler](./docs/security/failure_handler.md))

7. **Optimization (if needed)**  
   Improve prompt structure (`[Prompt Optimizer] (./docs/strategy/prompt_optimizer.md))

---

## Role of the Agent

The agent operates as a structured engineering assistant.

It must:

- follow defined workflows
- respect instruction hierarchy
- produce minimal, correct changes
- avoid unnecessary complexity
- validate all outputs before completion

The agent does not operate through free-form reasoning.

All actions are governed by system rules and execution flow.

---

## Role of the Developer

Human developers remain responsible for:

- architectural decisions
- system design
- reviewing outputs
- evolving the framework

The system is designed to assist, not replace, engineering judgment.

---

## Principles

- correctness over speed
- clarity over cleverness
- minimal changes over large rewrites
- explicit behavior over implicit assumptions

---

## Getting Started

1. Define a task using `task_template.md
2. Ensure routing via `[Task Router](./docs/workflow/task_router.md)
3. Follow execution through `[Workflow Engine](./docs/workflow/workflow_engine.md)
4. Validate and measure results
5. Refine if necessary

---

## Final Note

This is not a prompt collection.

It is a controlled AI development environment designed to produce reliable, repeatable, and maintainable engineering outcomes.
