# khanin-ch

Personal career data repository for **Khanin Chomphusri** — a single source of truth for all professional career information, designed to feed multiple downstream applications consistently and accurately.

## Purpose

This repository stores raw, comprehensive career data (work experience, projects, technical capabilities, education, etc.) that can be consumed by AI agents, tools, and applications without needing to maintain duplicate content across each one.

## Downstream Applications

| Application | Description |
|---|---|
| **[khanin.ch](https://khanin.ch)** | Personal portfolio website with AI-powered HR chatbot |
| **Resume Builder** | Generates tailored, ATS-optimized resumes based on a target job position |

## Repository Structure

```
docs/
  KNOWLEDGE_BASE.html          # Single source of truth — comprehensive career data
  KNOWLEDGE_BASE.css           # Stylesheet for the knowledge base HTML
resume_builder/
  RESUME_BUILDER_PROMPT.md     # Prompt for generating tailored, ATS-optimized resumes
  references/                  # Reference resume samples
```

## Design Principles

- **Raw data only** — no audience-specific narratives or tailored summaries; those belong in output layers
- **Evidence-backed** — every skill or claim links back to a specific project or role
- **AI-agent friendly** — structured HTML with semantic sections for easy parsing and querying
