# GVH 2026 評選平台 · Digital Judging System

> **Built with Vibe Coding** — Designed and product-managed by Jane Huang, MediaTek Internal Communications

🔗 **Live Demo**: https://janee1107.github.io/GVH_2026_Review/

---

## What is This?

The **GVH 2026 Review Platform** is a custom-built digital judging system for MediaTek's *Global Volunteer Hero Recognition* program — an internal award honoring employees who volunteer regularly and make a difference in their communities.

This platform replaced a manual, spreadsheet-based review process with a structured, data-driven experience for both internal and external judges.

---

## The Problem It Solves

| Before | After |
|--------|-------|
| Judges reviewed applications via email attachments | All applications accessible in one platform |
| Scores collected via Google Forms or Excel | Real-time scoring with progress tracking |
| No standardized rubric guidance | Built-in scoring rubric with level descriptions |
| Score aggregation done manually by coordinator | Automatic weighted score calculation + CSV export |
| Judges had no visibility into their progress | Live progress bar (0/40 applications reviewed) |

---

## Key Features

### 🏛️ Dual Access System
- **Internal judges** (MediaTek employees) and **external judges** authenticate separately
- Admin login for program coordinators to access the full dashboard

### ⚖️ Weighted Scoring Engine
Three evaluation dimensions with defined weights:
- **行動力 Action** · 40% — Commitment and consistency of volunteer efforts
- **影響力 Impact** · 35% — Measurable or qualitative change created
- **共鳴力 Resonance** · 25% — Ripple effect and inspiration to others
- **Long-term bonus** — +5 points for sustained service over 1 year

Each dimension includes a detailed 4-tier rubric (1–2 / 3–5 / 6–8 / 9–10) to ensure scoring consistency across judges.

### 📊 Real-Time Dashboard
- Live weighted ranking table across all applicants
- Internal / external judge scores combined at 50/50 weight
- Per-judge progress overview
- Judge comment aggregation by applicant

### 💾 Dual Data Strategy (Network-Aware)
The platform detects whether judges are on MediaTek's corporate network or personal WiFi and adapts:
- **Personal network**: Auto-sync to cloud, cross-device progress continuity
- **Corporate network (firewall)**: Manual CSV export with clear instructions

### 📁 Application Gallery
- Browse all 40 applications with filter (reviewed / unreviewed)
- Keyboard shortcuts for fast navigation (← → to switch, Enter to submit)
- AI preliminary report panel per application (internal reference)

---

## Technical Stack

| Layer | Technology |
|-------|------------|
| Frontend | Vanilla HTML / CSS / JavaScript |
| Data Storage | localStorage + Cloud sync (personal network) |
| Export | CSV generation via JS |
| Hosting | GitHub Pages |
| AI Integration | Connected to MediaTek internal Copilot (Jarvis) for pre-screening |

---

## How It Was Built

This platform was **100% product-managed and specification-written by Jane Huang** using a vibe coding approach — defining requirements, user flows, and edge cases through iterative dialogue with AI, then reviewing and validating the output.

No engineering team. No development budget. Built from scratch in weeks.

This project demonstrates:
- **Product thinking**: Identifying friction points in the existing process and designing solutions
- **User empathy**: Different flows for judges with different network environments
- **PM execution**: Turning fuzzy requirements ("we need judges to score applications") into a fully functional tool with edge case handling

---

## Context: The GVH Program

The Global Volunteer Hero Recognition is a MediaTek-wide CSR initiative celebrating employee volunteers. In 2026, the program received **40 applications** from employees across global offices. This platform supported the full judging lifecycle — from individual scoring to final weighted ranking.

---

*Built by Jane Huang · MediaTek Internal Communications · 2026*
