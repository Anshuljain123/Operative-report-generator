# Operative Report Generator

A browser-based AI clinical documentation tool built for a regulated pain management practice. Generates procedure-accurate Word documents with CPT auto-coding, conditional logic, and provider-specific defaults — no server required.

**Stack:** HTML · CSS · JavaScript · docx.js

---

## What It Does

Replaces manual operative report dictation and transcription with a structured, dropdown-driven interface that auto-generates a complete, formatted Word document on demand.

```
Physician selects procedure, side, levels, and provider settings
  → Conditional logic applies procedure-specific text, medications, and needle specs
  → CPT codes auto-populate based on selection
  → Word document (.docx) downloaded instantly in browser
```

---

## Procedures Covered (12 total)

| Category | Procedures |
|---|---|
| Cervical | CESI, SNRB, Medial Branch Block, Facet Joint Injection, RFA |
| Lumbar | LESI, Transforaminal ESI, SNRB, Medial Branch Block, Facet Joint Injection, RFA |
| Sacral | Sacroiliac Joint Injection (SIJ) |

---

## Features

- **CPT auto-coding** — correct codes auto-populate based on procedure, side, and number of levels (including add-on codes for multiple levels)
- **Conditional logic** — needle gauge/length, medication type/dose, procedural text, and attestation language all branch per procedure
- **DRL5 toggle** — switches needle length from 3½" to 5" where clinically indicated
- **IV sedation toggle** — bidirectional link with anesthesiologist dropdown (selecting Omar Othman M.D. auto-checks IV; unchecking sets Local Anesthesia Only)
- **Side/levels selection** — dynamic level options per procedure (cervical vs. lumbar anatomy)
- **Provider defaults** — dictating physician and anesthesiologist defaults configurable
- **Pure browser** — no server, no external API, no data leaves the device
- **Word output** — generates `.docx` using docx.js; compatible with Microsoft Word and Google Docs

---

## Clinical Context

**Problem:** Physicians and clinical staff spent 30+ minutes per shift on operative report documentation — manually selecting form variants from 45 source documents across 12 procedure types.

**Process:** Analyzed 45 operative report forms → extracted variable fields → built conditional logic per procedure → consolidated into a single parent application.

**Result:** Cleared a multi-month compliance backlog. Saves physicians 30+ minutes per shift. 100% adoption following physician UAT sign-off.

---

## Usage

Open `operative_report_generator.html` in any modern browser. No installation, no dependencies to install — docx.js loads from CDN.

---

## Built For

**Built for a regulated pain management clinic (Chicago, IL). Client name withheld.** · 
AI Implementation Consulting · Anshul Jain
