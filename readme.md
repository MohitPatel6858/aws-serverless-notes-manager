# AWS Serverless Notes Manager

A clean, professional frontend for a serverless notes app backed by **Amazon API Gateway**, **AWS Lambda**, **Amazon S3**, and monitored via **CloudWatch**.

This is a **frontend-only redesign**. No backend logic, request/response handling, or AWS integration was changed.

## What changed

- Rebuilt `index.html`, `style.css` from scratch in a light, minimal, Stripe/Linear/Notion-inspired style (previous version was a dark glassmorphism theme).
- New layout: sticky header → 4-stat dashboard → two-column Create/Read panels → full-width Recent Activity table.
- Palette, spacing, and component styling follow a professional SaaS dashboard aesthetic (see Design Tokens below).
- `script.js` logic is **unchanged**: same `API_BASE_URL`, same `fetch()` calls, same request bodies, same response handling, same DOM element IDs. The only addition is a small "Loaded" status badge and a footer wrapper in the read-result card markup — purely cosmetic, no behavior touched.

## What did NOT change

- `API_BASE_URL` and all fetch calls (`POST /note`, `GET /note?filename=...`)
- Request bodies and response parsing
- Validation, error handling, toast logic
- Statistics counting and animated counters
- Request history data model
- Element IDs referenced by JavaScript (`filenameInput`, `contentInput`, `saveBtn`, `readFilenameInput`, `readBtn`, `historyList`, etc.)

## Design tokens

| Token | Value |
|---|---|
| Background | `#F8FAFC` |
| Card | `#FFFFFF` |
| Primary | `#2563EB` |
| Success | `#16A34A` |
| Danger | `#DC2626` |
| Border | `#E5E7EB` |
| Text | `#111827` |
| Secondary text | `#6B7280` |

Fonts: **Inter** (UI text), **JetBrains Mono** (filenames, timestamps, response times, request history — anything that reads as data).

## Files

- `index.html` — markup
- `style.css` — styling
- `script.js` — application logic (unchanged behavior; same IDs as before)

## Setup

1. Open `script.js` and confirm `API_BASE_URL` points at your API Gateway stage:
   ```js
   const API_BASE_URL = "https://hmaue362a4.execute-api.ap-south-1.amazonaws.com";
   ```
2. Open `index.html` in a browser, or serve the three files from any static host (S3 + CloudFront, Amplify, Vercel, Netlify, etc.).
3. Create a note (writes to S3 via Lambda through API Gateway), then read it back by filename.

## Layout overview

```
┌─────────────────────────────────────────────────────────┐
│  Logo · Title / Subtitle        Status · Health · Clock │  sticky header
├─────────────────────────────────────────────────────────┤
│  [Total] [Successful] [Failed] [Notes Saved]             │  stat cards
├───────────────────────────┬───────────────────────────────┤
│  Create Note              │  Read Note                    │
│  - Filename                │  - Filename + Read button      │
│  - Content                 │  - Result card (filename,      │
│  - Save button              │    content, timestamp, badge)  │
├───────────────────────────┴───────────────────────────────┤
│  Recent Activity                                          │
│  Method | Filename | Status | Response Time | Time         │
└─────────────────────────────────────────────────────────┘
```