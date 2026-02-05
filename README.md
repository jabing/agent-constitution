# Agent Constitution ｜Agent 宪法系统
*A Deterministic, Model-Agnostic Multi-Agent Governance System*

---

## Introduction ｜ 简介

This repository is **not a prompt collection**.

Agent Constitution defines a **constitutional, role-separated, failure-aware multi-agent governance system** designed to prevent hallucination, role drift, and silent failure when working with large language models.

本项目并非 Prompt 拼装或 Agent Demo。  
它定义的是一套**宪法级、多角色分权、以失败为合法结果的 Agent 治理体系**，用于在复杂任务中约束大模型行为，避免幻觉、越权与“伪成功”。

---
## Constitutional Authority ｜ 宪法权威

This system is governed by a single constitutional document:

`governance/AGENT_CONSTITUTION.md`

It defines the **exclusive authority, responsibility boundaries, and failure signals**
for all agents in this system.

Any behavior, role definition, or workflow that conflicts with this constitution
is **invalid by definition**.

**Constitutional excerpt (authoritative):**

> Every role is intentionally incomplete.  
> Authority must be explicit, not inferred.  
> Failure is a legitimate outcome.  
> Termination is preferable to false success.  
> No role may both create and approve.

*Note:*  
The constitutional document is authored in Chinese to preserve precision.  
English explanations may be provided, but the Chinese version remains authoritative.


## Core Philosophy ｜ 核心理念

Agent Constitution is built on three non-negotiable principles:

1. **Verifiability over cleverness**（可验证性高于聪明）  
2. **Termination over false success**（终止优于错误完成）  
3. **Structure over improvisation**（结构优于即兴发挥）

The system treats multi-agent coordination as a **governance problem**, not a creativity problem.

---

## What This Is (and Is Not) ｜ 项目定位

### This project *is*
- A deterministic, role-governed multi-agent system
- Designed for auditability, boundary enforcement, and long-term stability
- Model-agnostic by design

### This project is *not*
- An AutoGPT-style autonomous agent framework
- A chat-based or conversational agent system
- A creativity or brainstorming tool

If you are looking for higher completion rates or more imaginative outputs, this is likely **not** the right system.

---

## Roles at a Glance ｜ 角色一览

| Role | Responsibility | Cannot Do |
|----|----|----|
| Analyst | Define problem boundaries | Propose solutions |
| Planner | Define verifiable tasks | Describe implementation |
| Implementer | Execute authorized tasks | Infer intent |
| Reviewer | Reject invalid work | Suggest fixes |
| Tester | Provide reproducible evidence | Speculate |
| CONDUCTOR | Final decision / termination | Participate in content |

Each role is deliberately **incomplete by design**.  
No role is allowed to be both creative and decisive.

---

## Agents Overview ｜ Constitutional View

Agents in this system are **not defined by capability**,  
but by **constitutional authority**.

Each agent exists to exercise a **strictly limited power**
granted by the constitution.
No agent is complete.
No agent is autonomous.
No agent may interpret its own authority.

The purpose of this design is not collaboration efficiency,
but **governance correctness**.

### Role Characteristics

- **Agents are incomplete by design**  
  Each agent is intentionally deprived of certain abilities
  to prevent silent escalation of authority.

- **Authority is exclusive, not shared**  
  If two agents appear capable of the same action,
  the system is misconfigured.

- **Failure is an explicit output**  
  Every agent has defined failure signals.
  Reporting failure is considered correct behavior.

- **No agent may approve its own work**  
  Creation and validation are constitutionally separated.

### Role Boundaries (Non-Exhaustive)

- **Analyst** defines problem boundaries and verifiability,
  but is forbidden from proposing solutions.

- **Planner** defines executable tasks,
  but is forbidden from describing how they are implemented.

- **Implementer** executes tasks exactly as specified,
  but is forbidden from expanding scope or intent.

- **Reviewer** validates compliance,
  but is forbidden from suggesting improvements.

- **Tester** provides reproducible evidence,
  but is forbidden from interpretation or speculation.

- **CONDUCTOR** decides continuation or termination,
  but is forbidden from participating in content.

These boundaries are **not conventions**.
They are enforced by the constitutional document.

Any behavior that crosses these boundaries
is invalid by definition.

---

## System Workflow ｜ 工作流程

Analyst → Planner → Implementer → Reviewer → Tester → CONDUCTOR

Rules:
- No backward flow  
- No role substitution  
- Only CONDUCTOR may end the process  

Failure is a valid and expected outcome at any stage.

---

## Model Compatibility ｜ 模型兼容性

Agent Constitution is **model-agnostic by design**.

It does not rely on any specific LLM architecture, toolchain, or execution framework.

The system has been **extensively validated** in OpenCode-style multi-agent orchestration environments and demonstrates particularly strong stability when used with DeepSeek models.

These environments are treated as **reference implementations**, not design dependencies.

---

## Repository Structure ｜ 仓库结构

agents/        # Role authority definitions  
governance/    # Constitution and final authority (CONDUCTOR)  
docs/          # Conceptual and onboarding materials  

Each file defines **authority boundaries**, not behavioral tips.  
If two files appear to overlap in responsibility, it is a bug.

---

## Getting Started ｜ 新手指引

1. Read `docs/PERSONA_PROFILES.md`  
2. Read `governance/AGENT_CONSTITUTION.md`  
3. Do **not** run anything yet  
4. Understand who is allowed to fail — and who must stop  

---

## Non-Goals ｜ 非目标

This system does **not** aim to:
- Maximize task completion rate
- Generate creative or conversational content
- Replace human judgment

Stopping is not a failure here.  
It is a safety mechanism.

---

## License & Citation ｜ 许可与引用

This project is released under the **Apache License 2.0**.

If you use this system in academic or engineering work, please see `CITATION.cff` for citation information.

> Agent Constitution does not try to make agents smarter.  
> It tries to make systems harder to break.

For rationale on constitutional language choice, see `docs/WHY_CHINESE_CONSTITUTION.md`.
