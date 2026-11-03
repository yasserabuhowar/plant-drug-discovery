# 🌿 PharmaScope — Plant-to-Drug Discovery Pipeline | منصة تحليل النباتات الدوائية

An Arabic-first research assistant that takes a medicinal plant and walks through a structured drug-discovery analysis: active compounds, molecular targets, development priorities, regulatory pathway, and links into 20 scientific databases.

مساعد بحثي عربي: تختار نبتة طبية فيعرض تحليلًا منظمًا من المركبات الفعالة حتى المسار التنظيمي، مع روابط مباشرة لقواعد البيانات العلمية.

---

## Two versions in this repo

| File | Version | How it works | Runs on GitHub Pages? |
|---|---|---|---|
| `index.html` | **v1 — Curated** | Hand-structured data for 6 plants (thyme, turmeric, black seed, ginger, chamomile, sage) | ✅ Yes |
| `ai.html` | **v2 — AI-powered** | Any plant name (Arabic / English / scientific) → Claude streams a 6-phase analysis | ⚠️ Only inside claude.ai (see below) |

## What the analysis covers

1. **Phytochemical profiling** — active compounds, chemical classes, extraction, top candidates
2. **Molecular targets** — protein/enzyme targets with evidence level, mechanisms, related diseases
3. **Drug pipeline** — prioritized therapeutic areas, timeline, Arab-region opportunity
4. **Research guide** — best databases, search terms, key journals
5. **Regulatory strategy** — FDA / EMA / WHO status, optimal pathway, IP, Palestinian and Arab regulatory gaps
6. **Live database links** — ChEMBL, PubChem, PubMed, UniProt, PDB, KEGG, DrugBank, ClinicalTrials.gov and 12 more

## Why

Most phytochemistry and drug-discovery tooling is English-only. This project explores how structured content and an LLM can give Arabic-speaking pharmacists and researchers a fast first pass on a plant before going to primary databases, with an explicit focus on regional regulatory context.

## Tech

- Single-file HTML / CSS / vanilla JavaScript, RTL layout, no build step, no dependencies
- v2: streaming LLM output (Claude) rendered phase by phase, with cancel support

## ⚠️ Known limitations

- **v2 AI calls** use the claude.ai Artifact runtime (`claude.use('sample')`). Outside claude.ai only Phase 6 works. Planned: a small backend proxy to the Claude API so it runs standalone without exposing an API key.
- **v1 reference list:** paper titles were drafted with AI assistance; the links are PubMed searches, not direct citations. Titles should be verified against PubMed before being cited.

## Disclaimer

For research and education only. Any real drug development requires validated laboratory and clinical studies and expert review.

## Author

**Yasser Abu Howar** — B.Pharm, MBA (Digital Business) candidate. Working at the intersection of pharmacy, regulation, and AI.
