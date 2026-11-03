# 🌿 Plant-to-Drug Discovery Pipeline | منصة تحليل النباتات الدوائية

An Arabic-first, AI-powered research assistant that takes the name of any medicinal plant (Arabic, English, or scientific name) and generates a structured six-phase drug-discovery analysis.

مساعد بحثي عربي مدعوم بالذكاء الاصطناعي: تُدخل اسم أي نبتة طبية فيُولّد تحليلًا منظمًا على ست مراحل، من المركبات الفعالة حتى المسار التنظيمي.

---

## What it does

| Phase | Output |
|---|---|
| 1. Phytochemical profiling | Active compounds, chemical classes, best plant part and extraction method, top 3 drug candidates |
| 2. Molecular targets | Reported protein/enzyme targets with evidence level, mechanisms, related diseases |
| 3. Drug pipeline | Three prioritized therapeutic areas, timeline, cost estimate, Arab-region opportunity |
| 4. Research guide | Most relevant databases, search keywords, key studies, specialist journals |
| 5. Regulatory strategy | FDA / EMA / WHO status, optimal regulatory pathway, IP landscape, Palestinian and Arab regulatory gaps |
| 6. Live database links | One-click searches in 20 databases (ChEMBL, PubChem, PubMed, UniProt, PDB, KEGG, DrugBank, ClinicalTrials.gov, etc.) |

## Why

Most phytochemistry and drug-discovery tooling is English-only. This project explores how an LLM can give Arabic-speaking pharmacists and researchers a fast, structured first pass on a plant before they go to primary databases, with an explicit focus on regional regulatory context.

## Tech

- Single-file HTML / CSS / vanilla JavaScript, RTL layout
- Streaming LLM output (Claude) rendered phase by phase, with cancel support
- No build step, no dependencies

## ⚠️ Current limitation

The AI phases (1–5) call Claude through the **claude.ai Artifact runtime** (`claude.use('sample')`). Opened anywhere else (for example GitHub Pages), only Phase 6 (database links) works and the page shows an "AI unavailable" notice.
Planned: a small backend proxy calling the Claude API so the page runs standalone without exposing an API key.

## Disclaimer

For research and education only. AI-generated content must be verified against primary literature; any real drug development requires validated lab and clinical studies.

## Author

**Yasser Abu Howar** — B.Pharm, MBA (Digital Business) candidate. Working at the intersection of pharmacy, regulation, and AI.
