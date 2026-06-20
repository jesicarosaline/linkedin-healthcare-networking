# LinkedIn Healthcare Networking Automation

**An AI-assisted outreach system for building a targeted professional network in U.S. healthcare growth.**

---

## What this project does

Breaking into a new industry from scratch is hard — especially when you don't have a ready-made network.

As a first-year MBA at Carnegie Mellon's Tepper School of Business, I'm targeting roles in **healthcare growth and strategy** in the U.S. Rather than send generic cold messages, I built a system that identifies the right people, verifies they're currently at active U.S. healthcare companies, and generates a personalized connection message for each one — then sends them automatically on a daily schedule.

The result: a structured, scalable outreach pipeline that reaches 20 new healthcare professionals per day with messages tailored to each person's company and role.

---

## What I built

### 1. Prospect list (243 contacts)
Scraped LinkedIn search results for people working in **growth roles at U.S. healthcare companies** — titles like VP of Growth, Chief Growth Officer, Head of Growth Strategy, and Director of Growth. Extracted name, title, and current employer for each person across multiple pages of search results.

### 2. Company research & categorization
For each of the 243 contacts, wrote a one-sentence description of their employer and categorized them by healthcare vertical:

| Category | Examples |
|---|---|
| AI / digital health | K Health, Twin Health, Hinge Health |
| Telehealth | Teladoc, MDI Health, Intercept Telehealth |
| Wellness & behavioral health | Grow Therapy, Strive Health, Tuesday Health |
| Health tech product | Tebra, Privia Health, Vatica Health |
| Healthcare finance & strategy | Healthcare Growth Partners, Sage Growth Partners |

### 3. Personalized outreach messages
Generated a custom ≤300-character LinkedIn connection message for every contact — referencing their specific company, tailored to my background (4 years in health startup growth in Indonesia + finance experience at EY and Medco), and written in a natural, non-salesy tone.

Message rules applied across all 243:
- ≤300 characters (hard limit for LinkedIn connection notes)
- No em dashes, no buzzwords, no generic openers
- Company name cleaned (no "LLC", "Inc.", "(Past)", etc.)
- Verified against a set of approved reference messages

### 4. Employment verification
Before sending to anyone, verified every contact is **currently** at a U.S. healthcare company by checking their LinkedIn Experience section — not just the job title in search results, which can be outdated.

Found and corrected 5 records where the company had changed:

| Person | Old record | Verified current employer |
|---|---|---|
| Evan M. | LettyAI (inactive) | Viper Partners |
| Nikhil M. | Silversmith Capital (past) | F-Prime |
| Adam V. | Providence (past) | Bon Secours Mercy Health |
| Shawn P. | Agape Care Group (past) | Innovation Healthcare Consulting |
| Mary Beth T. | New Innovations (past) | Ebix |

Removed 5 contacts whose current roles were outside U.S. healthcare (veterinary, general DTC brands, non-healthcare tech).

### 5. Automated daily sending
Set up a scheduled task that runs at 3PM ET every day. It finds the next 20 unsent contacts, injects personalized messages into LinkedIn's connection modal (via the Chrome extension + shadow DOM), sends each invitation, and logs the send date back to the Excel file.

---

## Files in this repo

| File | What it contains |
|---|---|
| `linkedin_growth_healthcare.xlsx` | Full contact list with names, titles, companies, descriptions, messages, and invitation send dates |
| `ai_task_log.xlsx` | Log of all AI-automated tasks used to build and maintain this project |

---

## Skills demonstrated

- **Workflow automation** — end-to-end pipeline from data collection to scheduled execution, with no manual steps after setup
- **Data quality** — employment verification loop that catches and corrects stale records before outreach
- **Personalization at scale** — 243 unique messages generated and validated against character limits and tone rules
- **Strategic networking** — structured approach to cold outreach in a target industry, with clear criteria for who qualifies

---

## Background

I'm Jesica Rosaline, an MBA student at Tepper (CMU) focused on healthcare growth strategy and AI implementation. Before Tepper, I spent 4 years in growth at a telehealth and wellness startup in Indonesia, and previously worked in strategy and transactions at EY, Helios Capital, and Medco.

This project is part of my effort to build genuine relationships with healthcare growth leaders in the U.S. while I'm in school.

📫 jrosalin@tepper.cmu.edu
