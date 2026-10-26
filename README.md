
# SENTINEL: LLM Failure & Safety Evaluation Lab

> **A human-in-the-loop (HITL) evaluation framework and dataset for identifying hallucinations, prompt-injection attacks, safety failures, compliance violations, and reliability issues in Large Language Models (LLMs).**

---

## 🎯 Project Overview

Standard AI benchmark datasets rely on simple binary tasks (positive/negative sentiment, cat vs. dog classification) that fail to test model robustness. **SENTINEL** is an advanced AI Quality Assurance (QA) and evaluation lab designed to stress-test LLMs against real-world failure modes.

Developed with a focus on **AI Safety, Governance, and Human-in-the-Loop (HITL) review standards**, this repository provides a production-grade annotation structure used by top AI evaluation platforms (OpenAI, Anthropic, Scale AI, Outlier, Labelbox).

---

## 📊 Core Failure Taxonomy

SENTINEL categorizes model degradation and failure vectors across 5 primary dimensions:

1. **Hallucination & Temporal Anachronism:** Inventing false facts, historical inaccuracies, or fabricating details about future events.
2. **Prompt Injection & System Leakage:** Overriding system guardrails, ignoring instructions, or leaking system prompts.
3. **Context Retention Failure:** Forgetting multi-turn conversational parameters or immediate user context.
4. **Ungrounded Summarization / Fabrication:** Introducing external claims or facts completely absent from the source document during summarization.
5. **Safety & Policy Violation:** Providing dangerous instructions, toxic content, or bypassing alignment guardrails.

---

## 🗂️ Repository Structure

```text
project-sentinel/
├── README.md                          # Master project documentation
├── configs/
│   └── label_studio_config.xml        # Custom Label Studio XML UI config
├── data/
│   └── sentinel_evaluation_sample.csv # Initial benchmark evaluation records
└── docs/
    └── annotation_handbook.md         # Severity scale and annotation guidelines
