# LinkedIn Healthcare Networking — Outreach Pipeline

**A structured, AI-assisted system for identifying and personalizing outreach to U.S. healthcare growth professionals.**

---

## What this project does

Breaking into a new industry from scratch is hard — especially when you don't have a ready-made network.

As a first-year MBA at Carnegie Mellon's Tepper School of Business, I'm targeting roles in **healthcare growth and strategy** in the U.S. Rather than send generic cold messages to anyone with a healthcare title, I built a pipeline that identifies the right people, scores and segments them by healthcare vertical, verifies their current employment, and generates a personalized outreach message for each one — so that every touchpoint is relevant and specific.

The result: a 243-person, fully enriched contact list with tailored messages, organized by category, and ready for a paced daily outreach cadence.

---

## What I built

### 1. Prospect identification (243 contacts)
Searched LinkedIn for people in **growth roles at U.S. healthcare companies** — titles like VP of Growth, Chief Growth Officer, Head of Growth Strategy, and Director of Growth. Extracted name, title, and current employer for each person.

### 2. Company research & segmentation
For each of the 243 contacts, wrote a one-sentence description of their employer and assigned them to a healthcare vertical based on company type:

| Segment | Examples |
|---|---|
| AI / digital health | K Health, Twin Health, Hinge Health |
| Telehealth | Teladoc, MDI Health, Intercept Telehealth |
| Wellness & behavioral health | Grow Therapy, Strive Health, Tuesday Health |
| Health tech product | Tebra, Privia Health, Vatica Health |
| Healthcare finance & strategy | Healthcare Growth Partners, Sage Growth Partners |

### 3. Personalized outreach messages
Generated a custom ≤300-character LinkedIn connection message for every contact — referencing their specific company, tailored to my background (4 years in health startup growth in Indonesia + finance experience at EY and Medco), and written in a natural, non-salesy tone.

Message rules enforced across all 243:
- ≤300 characters (LinkedIn connection note limit)
- No buzzwords, no generic openers
- Company name cleaned before use (no legal suffixes, no "(Past)" artifacts)
- Segment-specific templates — telehealth contacts get a different angle than finance contacts
- Verified against a set of approved reference messages for tone and length

### 4. Employment verification
Before finalizing anyone for outreach, verified that every contact is **currently** at a U.S. healthcare company — not just that they held a healthcare role at some point.

Found and corrected 5 records where the company had changed:

| Person | Stale record | Current employer |
|---|---|---|
| Evan M. | LettyAI (inactive) | Viper Partners |
| Nikhil M. | Silversmith Capital (past) | F-Prime |
| Adam V. | Providence (past) | Bon Secours Mercy Health |
| Shawn P. | Agape Care Group (past) | Innovation Healthcare Consulting |
| Mary Beth T. | New Innovations (past) | Ebix |

Removed 5 contacts whose current roles were outside U.S. healthcare (veterinary, general consumer brands, non-healthcare tech).

### 5. Outreach cadence design
Structured the contact list for a paced outreach cadence — 20 contacts per day, sequenced to avoid sending everything at once and allow time for responses before the next batch goes out. Each batch is pre-organized so outreach stays consistent without requiring daily re-prioritization.

---

## Files in this repo

| File | What it contains |
|---|---|
| `linkedin_growth_healthcare.xlsx` | Full contact list: names, titles, companies, segment categories, company descriptions, personalized messages, and outreach status |
| `ai_task_log.xlsx` | Log of all AI-automated tasks used to build and maintain this project |
| `growth_healthcare_li_skill/SKILL.md` | Reusable instructions for repeating this workflow on any new LinkedIn search — prospect extraction, enrichment, segmentation, message generation, and verification |

---

## Skills demonstrated

- **Lead scoring & segmentation** — categorized 243 prospects by healthcare vertical to match message angle to audience
- **Data quality** — employment verification loop that catches stale records before outreach goes out
- **Personalization at scale** — 243 unique messages generated and validated against character limits, tone rules, and segment-specific templates
- **Outreach strategy** — paced cadence design, structured pipeline with clear criteria for who qualifies and why
- **AI-assisted workflow design** — built a reusable skill that can reproduce this pipeline for any future search

---

## Background

I'm Jesica Rosaline, an MBA student at Tepper (CMU) focused on healthcare growth strategy and AI implementation. Before Tepper, I spent 4 years in growth at a telehealth and wellness startup in Indonesia, and previously worked in strategy and transactions at EY, Helios Capital, and Medco.

This project is part of my effort to build genuine relationships with healthcare growth leaders in the U.S. while I'm in school.

📫 jrosalin@tepper.cmu.edu
