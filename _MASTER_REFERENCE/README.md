# _MASTER_REFERENCE — Directory Guide

> **Created:** Feb 27, 2026 | **Last Updated:** Mar 8, 2026 | **Purpose:** Central hub for all indexes, keywords, prompts, guides, and reference materials used to pull information from multiple AI agents and manage the knowledge base.

---

## What This Folder Contains

### Core Reference Files

| File | Purpose |
|---|---|
| **PROJECT_BRIEFING.md** | Compact briefing document to onboard any new AI agent to the project instantly |
| **PROJECT_MISSION.md** | The central thesis, expanded mission, and philosophical framework for the entire project |
| **METHODOLOGY_AND_FACT_CHECKING.md** | Public-facing transparency document — tier system, [N/5] fact-checking, bias detection, quality metrics, limitations |
| **MASTER_INDEX.md** | Auto-generated index of all 1,071 research documents with tier, keywords, status |
| **KEYWORD_INDEX.md** | 17,185 unique keywords mapped to documents (22,995 keyword-doc links) |
| **SECTION_GUIDE.md** | Quick reference for what goes in each section (A–ZF, 32 sections) |
| **AI_SEARCH_GUIDE.md** | AI-optimized routing document — read FIRST to find the right docs for any query |

### Workflow & Prompts

| File | Purpose |
|---|---|
| **AI_AGENT_PROMPTS.md** | All prompt templates for pulling research from Claude, GPT, Gemini, and other AI agents |
| **RESEARCH_METHODOLOGY.md** | Tier system, source hierarchy, bias flags, interpretive lenses, quality standards |
| **STYLE_GUIDE.md** | Formatting rules, template structure, naming conventions |

### Maps & Planning

| File | Purpose |
|---|---|
| **CONNECTED_TOPICS_RESEARCH_MAP.md** | Maps 20+ thematic threads, 200+ cross-domain connections across the full corpus |

---

## How To Use This Folder

### Starting a Research Session
1. Open **PROJECT_BRIEFING.md** — copy it into any AI agent to give full context
2. Check **CONNECTED_TOPICS_RESEARCH_MAP.md** — pick a topic to work on
3. Copy the appropriate prompt from **AI_AGENT_PROMPTS.md**
4. Fill in the topic and run across multiple AI agents
5. Create the document following **STYLE_GUIDE.md**
6. Update indexes (or run the pipeline in `_scripts/`)

### Onboarding a New AI Agent
1. Paste **PROJECT_BRIEFING.md** into the agent
2. Paste **RESEARCH_METHODOLOGY.md** for quality rules
3. Paste the relevant prompt from **AI_AGENT_PROMPTS.md**
4. The agent now has full context to contribute

### Finding Connections
1. Open **CONNECTED_TOPICS_RESEARCH_MAP.md**
2. Search for your topic in the connection tables
3. Follow cross-references to related documents
4. Use the MEGA-CONNECTIONS section for deep synthesis

### Running the Pipeline
1. See `_scripts/HOW_TO_USE.md` for setup instructions
2. Run `python _scripts/run_pipeline.py` to regenerate MASTER_INDEX and KEYWORD_INDEX
3. Copy updated indexes to this folder

---

*This folder is the brain of the project. Keep it updated.*
