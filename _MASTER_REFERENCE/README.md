# _MASTER_REFERENCE — Directory Guide

> **Created:** Feb 27, 2026 | **Last Updated:** Mar 14, 2026 | **Purpose:** Central hub for all indexes, keywords, prompts, guides, and reference materials used to pull information from multiple AI agents and manage the knowledge base.

---

## What This Folder Contains

### Core Reference Files

| File | Purpose |
|---|---|
| **PROJECT_BRIEFING.md** | Compact briefing document to onboard any new AI agent to the project instantly |
| **PROJECT_MISSION.md** | The central thesis, expanded mission, and philosophical framework for the entire project |
| **METHODOLOGY.md** | Research methodology, document structure, interpretive frameworks, transparency |
| **FACT_CHECKING.md** | Verification systems, scoring metrics, external APIs, bias detection, quality metrics |
| **MASTER_INDEX.md** | Auto-generated index of all 2,437 research documents with tier, keywords, status |
| **KEYWORD_INDEX.md** | 30,579+ unique keywords mapped to documents |
| **SECTION_GUIDE.md** | Quick reference for what goes in each section (A–ZH, 34 sections) |
| **AI_SEARCH_GUIDE.md** | AI-optimized routing document — read FIRST to find the right docs for any query |

### Workflow & Prompts

| File | Purpose |
|---|---|
| **AI_AGENT_PROMPTS.md** | All prompt templates for pulling research from Claude, GPT, Gemini, and other AI agents |
| **STYLE_GUIDE.md** | Formatting rules, template structure, naming conventions |
| **SYSTEM_REVIEW.md** | System health check, keyword coverage, pipeline status, expansion readiness |

### Maps & Planning

| File | Purpose |
|---|---|
| **CONNECTED_TOPICS_RESEARCH_MAP_v7.md** | Maps 20+ thematic threads, 200+ cross-domain connections across the full 2,437-doc corpus |

---

## How To Use This Folder

### Starting a Research Session
1. Open **PROJECT_BRIEFING.md** — copy it into any AI agent to give full context
2. Check **CONNECTED_TOPICS_RESEARCH_MAP_v7.md** — pick a topic to work on
3. Open `_scripts/prompts/research_pull_prompt.md` — this is the **CANONICAL prompt** for creating new documents. Copy the "Universal Research Pull" section, replace `[TOPIC]` and `[SECTION_ID]`, and paste into any AI agent
4. For quick expansions of existing docs, use the "Quick-Pull Variant" from the same file
5. Create the document following **STYLE_GUIDE.md**
6. Update indexes (or run the pipeline in `_scripts/`)

> **Important:** Do NOT use the abbreviated prompts in AI_AGENT_PROMPTS.md §2-3 for document creation — they redirect to the canonical prompt. The single source of truth for document creation is `_scripts/prompts/research_pull_prompt.md`.

### Onboarding a New AI Agent
1. Paste **PROJECT_BRIEFING.md** into the agent
2. Paste **METHODOLOGY.md** and **FACT_CHECKING.md** for quality rules
3. For new document creation: use `_scripts/prompts/research_pull_prompt.md` (the canonical prompt)
4. For verification: use `_scripts/prompts/source_verification_prompt.md` or `_scripts/prompts/comprehensive_quality_sweep_prompt.md`
5. The agent now has full context to contribute

### Finding Connections
1. Open **CONNECTED_TOPICS_RESEARCH_MAP_v7.md**
2. Search for your topic in the connection tables
3. Follow cross-references to related documents
4. Use the MEGA-CONNECTIONS section for deep synthesis

### Running the Pipeline
1. See `_scripts/HOW_TO_USE.md` for setup instructions
2. Run `python _scripts/pipeline.py` to regenerate MASTER_INDEX and KEYWORD_INDEX
3. Copy updated indexes to this folder

---

*This folder is the brain of the project. Keep it updated.*
