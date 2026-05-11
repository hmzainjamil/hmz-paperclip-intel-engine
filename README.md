# hmz-paperclip-intel-engine

> **Autonomous competitor intelligence + market signal engine | runs 10:00 AM daily | DigiMinds strategic awareness**

[![schedule](https://img.shields.io/badge/schedule-10%3A00AM_daily-blue?style=flat)](.) [![intel](https://img.shields.io/badge/output-competitor_intel-red?style=flat)](.) [![status](https://img.shields.io/badge/status-always_on-brightgreen?style=flat)](.) [![company](https://img.shields.io/badge/company-DigiMinds-orange?style=flat)](.)

[Overview](#overview) · [Sources](#sources) · [Signals](#signals) · [Output](#output) · [Tips](#tips)

---

## 🧠 OVERVIEW

Paperclip Intel Engine scans the competitive landscape every morning at 10 AM. It monitors competitor ad activity, pricing changes, new service launches, client wins/losses, and platform policy changes that could affect DigiMinds positioning. Results feed directly into CEO loop context.

| Component | Value |
|---|---|
| Trigger | Daily 10:00 AM (LaunchAgent) |
| Scope | Top 10 PPC agency competitors + Google/Meta platform changes |
| Model | Groq Llama 3 + Gemini Flash (zero Claude tokens) |
| Output | Intel brief → Paperclip API → CEO loop context |

---

## ⚙️ SOURCES MONITORED

| Source | Signal | Method |
|---|---|---|
| Google Ads Transparency Center | Competitor ad creative changes | Apify actor |
| Meta Ad Library | Competitor Facebook/Instagram ads | Apify actor |
| LinkedIn | New hires, job posts, service updates | Apify scraper |
| Google News | Agency news, PPC industry updates | News API |
| SimilarWeb (public) | Competitor traffic trends | Apify |
| Agency websites | Pricing, service page changes | Diff monitoring |
| Clutch.co | New reviews on competitor profiles | Scraper |

---

## 🎯 SIGNAL TYPES

| Signal Type | Meaning | Priority |
|---|---|---|
| Competitor drops price | Market pressure — review DigiMinds pricing | HIGH |
| Competitor launches new service | Potential gap in DigiMinds offer | HIGH |
| Platform policy change (Google/Meta) | Client campaigns need updating | CRITICAL |
| Competitor loses major client | Outreach opportunity | MEDIUM |
| Competitor hires senior talent | They're scaling — watch closely | MEDIUM |
| New entrant to market | Landscape shift — update ICP | MEDIUM |

---

## 💡 TIPS

■ **Intelligence Quality (4)**
| Tip | Source |
|---|---|
| Meta Ad Library is the most reliable competitor signal — check ad volume changes | Intel SOP |
| Google Ads Transparency shows exact competitor messaging angles to counter | PPC playbook |
| Clutch reviews reveal competitor weaknesses — mine them for sales ammo | Sales SOP |
| Platform policy changes need same-day CEO loop escalation — never wait | Operations rule |

■ **Operations (3)**
| Tip | Source |
|---|---|
| Intel brief is stored at `/api/intel/latest` — CEO loop reads it every 6h | API ref |
| Historical intel at `/api/intel?days=30` shows trend lines | API ref |
| Custom competitor can be added via `/api/intel/competitors/add` | API ref |

---

## ☠️ TOOLS REPLACED

| Intel Engine | Replaced |
|---|---|
| Competitor monitoring | Manual weekly reviews |
| Ad library checks | Manual ad library browsing |
| Platform policy tracking | Forgetting to check until client complains |
| Market signal detection | Gut feeling |

---

*Part of [DigiMinds AI Agency Stack](https://github.com/hmzainjamil) — Paperclip autonomous intelligence*
