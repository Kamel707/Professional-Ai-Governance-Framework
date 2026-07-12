# Professional AI Governance Framework

[![License: CC BY-ND 4.0](https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nd/4.0/)
[![Status](https://img.shields.io/badge/status-stable-brightgreen.svg)]()

**A governance framework for the professional use of AI — designed for any regulated practice (engineering, law, medicine, finance).**

This repository contains a ready-to-use **Claude Skill**: it structures the collaboration between a responsible professional and an AI assistant around validation gates, a criticality classification, and a normative framing mechanism that prevents the AI from asserting that a standard or reference framework applies without human confirmation.

Developed and generalized from the *SYVEX AI Framework*, used in production in geotechnical and structural engineering by [SYVEX ENGINEERING](https://github.com/Kamel707) / SYVEX AI Solutions.

---

## Why this framework

Using generative AI within a regulated professional practice carries a simple but serious risk: AI can produce a plausible but unverified result, with a confidence level that does not reflect its actual reliability. This framework does not aim to restrict AI use — it structures it so that **final responsibility and decision-making always stay in the professional's hands**.

Key principles:
- AI never decrees that a reference framework (standard, code, guideline) applies — it questions the professional and documents the answer.
- Every deliverable is classified by criticality level (N1 to N4), with a proportionate validation requirement.
- Moving from one project stage to the next is conditioned by explicit validation gates (G0 to G5).

---

## Repository contents

| File | Role |
|---|---|
| `SKILL.md` | The Skill content: principles, G0 framing mechanism, G0–G5 gates, N1–N4 classification, source registry, sectoral examples. |
| `LICENSE.md` | Creative Commons Attribution – No Derivatives license (CC BY-ND 4.0). |
| `CHANGELOG.md` | Version history of this Skill. |
| `README.md` | This file. |

---

## Installation — using this Skill with Claude

1. Download `SKILL.md` from this repository.
2. Place the file in your Claude environment's skills folder:
   - **Claude Code**: `.claude/skills/professional-ai-governance/SKILL.md` at your project's root.
   - **Claude.ai / Cowork**: add the file through your project's Skills management, if available on your plan.
3. Once loaded, the Skill activates automatically whenever a task matches its description (producing a deliverable that carries professional responsibility).

No external dependency is required — the file is a standalone Markdown document.

---

## What this Skill is not

- It is **not** a collaborative open source project: contributions, modifications and redistribution of modified versions are not permitted (see license).
- It is **not** executable software: it is a methodological framework consumed by an AI assistant.
- It does **not replace** a professional reference framework, a technical standard, or the judgment of a qualified professional.

---

## Going further

The full version applied to engineering (filled-in templates, quantified KPIs, real registries, the GeoLab CBR application example) remains a proprietary development of SYVEX ENGINEERING. For questions, collaboration, or an in-depth demonstration, contact the author.

**Author:** Kamel Bouadel — SYVEX ENGINEERING / SYVEX AI Solutions
📩 Contact: bouadelfk@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/kamel-bouadel-195b37388

---

## License

This repository is published under the **CC BY-ND 4.0** license — free use with mandatory attribution, no modifications permitted. See [LICENSE.md](./LICENSE.md).
