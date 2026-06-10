# Ash Inglis Psychology — Website & Business Infrastructure Project

> **Status:** In planning / early build phase  
> **Last updated:** June 2026  
> **Project type:** Professional website + business workflows for a new psychological assessment practice

---

## Overview

This repository contains the website and supporting materials for **Ash Inglis Psychology**, a psychological assessment practice based in **Darwin, Northern Territory, Australia**.

The project goal is to establish a professional web presence and supporting business workflows that serve three distinct client streams: government and criminal justice bodies, health professionals, and individuals (including NDIS participants).

---

## About the Practice

| Detail | Info |
|---|---|
| **Psychologist** | Ash Inglis |
| **AHPRA Registration** | To be confirmed |
| **Location** | Darwin, Northern Territory |
| **Service area** | Darwin (in-person) + NT-wide via Telehealth |
| **Telehealth** | Available across remote NT communities |

---

## Client Streams

The website and referral pathways are structured around **three distinct referrer types:**

### 1. Organisations & Government
- Government agencies
- Criminal justice system (corrections, courts, legal representatives)
- NDIS providers
- Corporate employers

**Services include:** fitness for duty assessments, pre-employment psychological screening, court-ordered assessments, medico-legal reports, risk assessments.

### 2. Health Professionals
- GPs
- Psychiatrists
- Mental health teams (public and private)

**Services include:** diagnostic assessments, cognitive assessments, treatment planning profiles, standardised reporting.

### 3. Individuals & Families
- Self-referrals
- Private patients
- NDIS participants

**Services include:** functional capacity assessments, psychosocial disability assessments, support needs assessments, diagnostic assessments, NDIS evidence reports.

---

## Website Design Direction

### Style & Tone
- **Tone:** Professionally warm — trustworthy, calm, approachable. Not cold or overly clinical.
- **Palette:** Muted earth tones (warm slate, ochre, cream, sand) — avoiding clinical blues; suited to the NT context
- **Typography:** Clean sans-serif for body text (Inter); warmer serif for headings (Lora)
- **Imagery:** Clean and respectful. No cliché stock imagery. No generic "outback" visuals.

### Homepage Layout
The homepage uses a **three-pathway split** — the primary design decision. Visitors are immediately directed to one of three streams:

- → Organisations & Government
- → Health Professionals
- → Individuals & Families

Each pathway leads to tailored content, a tailored referral form, and stream-specific service information.

### Key Sections
- Crisis support bar (top — emergency numbers)
- Contact bar (phone, email, telehealth availability)
- Sticky navigation
- Hero section with NT-specific messaging
- Acknowledgement of Country ribbon (prominent placement — not buried in footer)
- Three-way gateway (referrer pathway selector)
- Cultural safety block
- Assessment pipeline (what to expect: intake → interview → testing → report)
- About Ash section
- Secure referral form (conditional logic by referrer type)
- Footer with Acknowledgement of Country, links, emergency contacts

---

## Cultural Safety — Non-Negotiable Elements

Given the Darwin/NT context and the likely First Nations client base across all streams:

- **Acknowledgement of Country** — Larrakia People, Darwin. Displayed prominently (ribbon placement below hero, and again in footer).
- **Cultural safety statement** — Genuine commitment to respectful, responsive, culturally safe practice for First Nations individuals and families across the Top End.
- **Interpreter services** — Aboriginal Interpreter Services (AIS) and national translation networks. Noted on both the cultural safety section and the referral form.
- **Remote community access** — Telehealth services explicitly flagged for remote NT communities.

---

## Referral Form — Field Logic

The referral form uses a **conditional field structure** based on referrer type. A dropdown at the top — *"I am referring as…"* — shows and hides relevant fields.

### Fields shown for all referrers:
- Referrer name, organisation, contact details
- Client name, date of birth, contact details
- Reason for referral / specific assessment questions
- Assessment urgency (routine / urgent)
- Funding pathway (Government, NDIS, Private, Medicare, Legal)
- Interpreter required? (Yes / No)
- Remote community? (Yes / No)
- Preferred mode (in-person Darwin / Telehealth)
- Document upload (referral letter, court order, NDIS plan)

### Additional fields — Health Professionals:
- GP provider / Medicare number
- Relevant diagnostic queries
- Mental Health Care Plan attached?

### Additional fields — Government / Legal:
- Court / matter reference number
- Instructing party / legal firm
- Report deadline

### Additional fields — Individuals / NDIS:
- NDIS participant number
- Plan manager contact details
- Plan management type (self / plan / NDIA managed)

---

## Recommended Tech Stack

| Function | Recommended Tool | Notes |
|---|---|---|
| **Website** | Webflow | Visual editor, no coding required, professional output |
| **Referral forms** | JotForm (healthcare compliance tier) | HIPAA/healthcare compliant, conditional logic, email integration |
| **Practice management** | Halaxy | Built for Australian Allied Health; handles Medicare, NDIS billing, scheduling |
| **Domain registration** | VentraIP or Crazy Domains | Australian registrars; `.com.au` and `.au` domains |
| **Prototype / staging** | GitHub Pages | Current prototype hosted here |

---

## NT-Specific Considerations

- **Timezone:** ACST (UTC+9:30) — note on contact page for interstate referring organisations
- **Telehealth:** Must be prominent throughout — Darwin's catchment includes remote NT communities
- **Cultural safety:** Not a checkbox; a genuine practice commitment reflected throughout the site
- **Interpreter services:** Flag availability early — relevant to criminal justice, NDIS, and mental health streams
- **AHPRA number:** To be displayed in footer once confirmed

---

## Current Build Status

| Item | Status |
|---|---|
| Project scoping | ✅ Complete |
| Client stream definition | ✅ Complete |
| Design direction | ✅ Complete |
| HTML prototype | ✅ Live on GitHub Pages |
| Referral form (conditional logic) | ✅ In prototype |
| About Ash content | ⏳ Awaiting copy from client |
| AHPRA registration number | ⏳ To be confirmed |
| Real phone number | ⏳ To be confirmed |
| Production build (Webflow) | 🔲 Not started |
| JotForm backend | 🔲 Not started |
| Halaxy setup | 🔲 Not started |
| Domain registration | 🔲 Not started |

---

## On the Horizon

1. Migrate prototype to Webflow for production build
2. Set up JotForm (healthcare tier) as the secure referral form backend
3. Register Australian domain via VentraIP or Crazy Domains
4. Set up Halaxy as practice management system
5. Populate "About Ash" section with real bio copy and photo
6. Confirm and add AHPRA registration number
7. Add fees and funding pathways page
8. Add privacy policy page (required — health data)

---

## Repository Structure

```
/
├── index.html          # Main prototype (currently live on GitHub Pages)
└── README.md           # This file
```

---

## Notes for Editors

- The prototype is a **single-file HTML build** — all CSS and JS is inline in `index.html`
- To make edits without coding: paste the file content to Claude for assisted changes, or use the GitHub browser editor for simple text updates
- The referral form in the prototype is **UI only** — it does not yet submit data anywhere. Backend (JotForm) to be connected in production build.

---

*Project managed by Tanya on behalf of Ash Inglis Psychology.*
