

## 📌 Overview

This repository contains an in-depth business information systems analysis of **Spotify Technology S.A.**, exploring the layered digital infrastructure that powers one of the world's largest music streaming platforms. Rather than focusing on Spotify's content catalogue, the report examines *how the company's systems work together* — from a single tap-to-play event, through royalty processing, to the algorithms behind Discover Weekly — to create a data-driven competitive moat.

The analysis is grounded in the **Data → Information → Knowledge → Wisdom (DIKW) hierarchy** and maps Spotify's operations onto standard Business Information Systems categories (TPS, MIS, DSS, Enterprise Systems, and E-Business Platforms).

---

## 📖 Table of Contents

1. [Organisation Overview](#1-organisation-overview)
2. [Information and Decision-Making](#2-information-and-decision-making)
3. [Business Information Systems Analysis](#3-business-information-systems-analysis)
4. [Digital Business Workflow Analysis](#4-digital-business-workflow-analysis)
5. [Strategic Advantage through Digital Business](#5-strategic-advantage-through-digital-business)
6. [Challenges and Recommendations](#6-challenges-and-recommendations)
7. [Conclusion](#conclusion)
8. [Authors](#-authors)

---

## 1. Organisation Overview

Spotify was founded in 2006 in Stockholm, Sweden, and its parent company, **Spotify Technology S.A.** (Luxembourg), went public on the NYSE in 2018 via a direct listing — a rare choice that signaled the brand's confidence in its market visibility.

- **Business model:** A two-sided marketplace connecting listeners on one side with artists, labels, and advertisers on the other, operating on a **freemium** revenue model (Premium subscriptions + ad-supported free tier).
- **Digital ecosystem:** Spans the core streaming app, *Spotify for Artists*, integrations with Apple CarPlay and Amazon Alexa, and a backend built on **Google Cloud Platform (GCP)**, **Kafka** (real-time event streaming), and **Cassandra** (distributed data storage).
- **Customer segments:** Listeners, podcast creators, artists/labels, and advertisers — each with distinct, sometimes conflicting, system requirements.

## 2. Information and Decision-Making

The report applies the **DIKW hierarchy** to Spotify's operations:

| Layer | Example at Spotify |
|---|---|
| **Data** | Raw logs of plays, skips, pauses, and listening duration |
| **Information** | Aggregated trends — which songs/genres are trending by region |
| **Knowledge** | Patterns discovered via ML — e.g., genre preferences shifting by time of day |
| **Wisdom** | Strategic action — building Discover Weekly, launching new features |

**Types of data generated:** Behavioural (streams, skips, saves), Contextual (device, location, time), Content metadata (genre, tempo, mood), and Financial (subscriptions, ad revenue, royalties).

## 3. Business Information Systems Analysis

The report traces how information flows through five interconnected system layers:

```
User Activity → TPS → MIS → DSS → Enterprise Systems → E-Business Platform → User Experience
```

- **TPS (Transaction Processing Systems):** Captures real-time events — streams, payments, ad delivery.
- **MIS (Management Information Systems):** Converts TPS data into reports for engagement analysis and royalty tracking.
- **DSS (Decision Support Systems):** Powers recommendation engines, churn prediction, and retention strategy.
- **Enterprise Systems:** Integrates outputs into finance, HR, and rights management.
- **E-Business Platforms:** The consumer-facing layer — app, artist tools, and advertising products.

## 4. Digital Business Workflow Analysis

Three key workflows are broken down step-by-step:

### 🎵 Song Streaming — Tap to Audio
Local cache check → session/licensing verification → CDN edge routing → chunked audio delivery (~200ms to first sound) → stream-event logging (royalty trigger at 30s) → background pre-loading of the next track.

### 🎧 Discover Weekly — Data to Playlist
Weighted behavioral signals (skips vs. completions) → collaborative filtering (similar users) → content-based filtering (audio features) → NLP on cultural context (blogs, playlist descriptions) → ranking model narrows candidates to 30 → pre-built and cached every Sunday night.

### 👋 New User Onboarding — Sign-Up to Taste Profile
Genre/artist picks map to a taste-embedding space → "borrowed" behavior from similar users solves the cold-start problem → home screen personalizes instantly → real interactions gradually overwrite borrowed signals.

## 5. Strategic Advantage through Digital Business

Since music catalogues are largely identical across platforms, Spotify's edge comes from **how it uses data and systems**, not the content itself:

- **i. Personalisation** — Discover Weekly, Daylist, and other ML-driven features that compound in value with more listening data.
- **ii. Customer retention** — Spotify Wrapped and daily personalized playlists as low-cost, high-engagement retention tools.
- **iii. Scalability** — Cloud-native architecture enabling global growth without proportional infrastructure cost.
- **iv. Automation** — Royalty processing and rights management automated across millions of tracks.
- **v. Two-sided platform value** — Spotify for Artists deepens supply-side lock-in via analytics tools.
- **vi. Freemium conversion** — Free tier as an acquisition funnel, backed by data-driven upgrade prompts.

## 6. Challenges and Recommendations

**Key challenges identified:**

- **Security** — vulnerability to credential stuffing and fake stream manipulation (bot-driven royalty/chart inflation).
- **Privacy** — balancing rich personalization against GDPR, India's DPDPA, and other evolving regional regulations.
- **Data management** — maintaining consistency across TPS, MIS, and recommendation systems to avoid royalty/stream-count discrepancies.

**Recommendations proposed:**

- Periodic cross-system **data reconciliation checks** for royalty and billing accuracy.
- **Expanded UI personalization** — custom color themes, including mood-adaptive theming based on listening habits.
- **Simplified playlist navigation** — undo/trash-bin for deleted playlists, fewer steps to create a playlist.
- **AI-assisted playlist naming** based on the mood/genre/vibe of tracks in a playlist.

## Conclusion

Spotify's success lies not in owning music, but in mastering the **systems that move it**. From the play button to royalty payment, layered information systems convert raw data into decisions, personalization, and revenue. As the streaming market grows more crowded, security, privacy, and data integrity will matter as much as recommendation algorithms — making continued investment in robust information systems central to Spotify's competitive future.

---

## 📁 Repository Contents

| File | Description |
|---|---|
| `Digital_business_system_CIA1.docx` | Full report submission |
| `README.md` | This file |

## ✍️ Authors

- Erin Braggs
- Manmeet Kaur Oberoi
- Siya Anand
- Srinidhi Susarla
- Udditee Kapoor

---

