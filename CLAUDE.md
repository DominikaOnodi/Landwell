# CLAUDE.md — Landwell Project Context

> This file is automatically read by Claude Code at the start of every session.
> Do not delete it. Update the Progress Log after each coding session.

---

## Project Overview

**Platform name:** Landwell  
**Tagline:** *A borderless community for people building life abroad*  
**Type:** Human-centered relocation and international living platform  
**MVP city:** London (architecture must support adding more cities later)

This is NOT a corporate relocation platform. The entire experience should feel like a trusted friend helping you navigate a new city — warm, emotionally supportive, community-oriented, and culturally curious.

---

## Founder Context

- Solo founder, beginner developer
- Basic familiarity with HTML/CSS, learning Python (data science)
- No prior experience with JS frameworks or deployment
- Please explain decisions clearly, avoid jargon without explanation
- Work step by step — do not generate large amounts of code at once
- Wait for confirmation before moving between sections

---

## Brand Identity

### Color Palette
- Background: warm cream / off-white `#F5F0EA`
- Primary: deep sage green `#3D5A40`
- Accent: terracotta / burnt orange `#C87941`
- Text: dark warm brown / near-black
- Decorative: small hearts ♥ and sparkle ✦ motifs used sparingly

### Typography Feel
- Warm, editorial, slightly rounded — not corporate sans-serif
- Avoid: Inter, Roboto, Arial, generic system fonts
- Aim for: something distinctive, readable, emotionally warm

### Logo Elements
- Arched doorway (sage green) = arrival, new beginnings
- Rising sun (terracotta) behind a gentle hill
- Winding path leading to the door
- Small sparkle/star accents
- Wordmark: "Landwell" — elegant but approachable

### Overall Aesthetic
- Warm cream backgrounds with sage + terracotta accents
- Rounded UI elements
- Generous whitespace
- Subtle hover interactions and motion
- Small decorative hearts/sparkles used meaningfully
- Mobile-first always
- Inspired by: Kinfolk magazine meets a warm community app
- Avoid: corporate SaaS, purple gradients, cold startup aesthetics

---

## The Three Mascots

All mascots are **round, soft, expressive illustrated potato characters**. Same visual style across all three — warm potato energy, different accessories.

### 🥔 The Explorer
- Wears a backpack, holds a map with a small heart on it
- Curious, friendly, always discovering
- **Covers:** city discovery, culture, cafés, museums, events, hidden gems, local recommendations, weekly city guides
- **Tone:** playful, curious, adventurous

### 🥔 The Settler
- Sits comfortably with a warm mug, small plant nearby
- Finding comfort, building routines, creating home
- **Covers:** relocation support, moving checklists, visa guidance, healthcare, banking, renting, bureaucracy, insurance, jobs, practical settling-in info
- **Tone:** calming, reassuring, supportive

### 🥔 The Connector
- Holds a heart flag, carries a small shoulder bag
- Bringing people together, building community
- **Covers:** meeting people, events, internationals network, language exchanges, creative meetups, local gatherings, friendships, shared journeys
- **Tone:** warm, social, welcoming

---

## Site Architecture (MVP)

### Homepage Sections (in order)
1. Hero — emotional headline, tagline, warm visual, CTA
2. Mission — brief, human, warm. Why Landwell exists.
3. Mascot introduction cards — one per mascot, visually charming
4. Section previews — Explorer / Settler / Connector
5. Instagram / social links
6. Newsletter signup (placeholder, not functional yet)
7. Footer — simple, warm

### Future Sections (placeholder only — do not build yet)
- Interactive map (city-based, expandable)
- Relocation checklists (visa, first week, banking, healthcare)
- Events listings
- Local city guides
- Community / connection spaces
- AI relocation assistant

---

## Tech Stack
*(Update this section once stack is confirmed in first session)*

- Framework: TBD
- Styling: TBD
- Hosting: TBD
- Notes: must be beginner-friendly, mobile-first, scalable

---

## How We Work Together

- Always read this file at the start of a new session
- Summarize current project state before suggesting next steps
- Build one section at a time, confirm before moving on
- Explain decisions in plain language
- Keep code organized with clean folder structure
- Prioritize mobile-first, responsive design at every step

---

## Progress Log

> Update this section manually at the end of each coding session.
> Format: `- [Section/feature] — [status] — [date]`

### Completed
- Hero section — full-height opening, arch SVG icon, headline, CTAs — session 1
- Global design tokens, fonts (Cormorant Garamond + DM Sans), button styles, layout utils — session 1
- Nav component — fixed top bar, logo + links — session 1
- Mascots section — three clickable cards (Explorer, Anchor, Connector) with inline SVG potato characters — session 2
- Globe/map section — animated CSS spinning globe, London pin with pulse, coming-soon city chips — session 2
- Mission section — personal origin story, centered italic heading, warm prose, sage-pale background — session 2
- Portals redesigned as primary navigation / hero — arch shape, mix-blend-mode images, now first on page — session 3
- Hero section removed — brand tagline absorbed into portals header — session 3
- Three mascot pages built (/explorer, /anchor, /connector) — shared MascotPage layout, globe + category cards — session 3
- Architecture confirmed: mascot-first routing, globe as city selector within each mascot's page — session 3
- Dubai city page (/dubai) — dark desert hero, custom skyline SVG, stat chips, guide card grid — session 4
- Dubai globe pin — activated as second live city alongside London — session 4
- Dubai Anchor guides — /dubai/visas, /dubai/renting, /dubai/banking — full content — session 4
- All mascot PNGs dropped into public/mascots/ (explorer, anchor, connector + page-specific variants) — session 4
- Footer component — simple, warm — session 4
- Instagram links — linked in footer/nav — session 4
- Connector portal colour updated — changed from cream-dark to mint-pale (#DFF2E6) to distinguish from background — session 4

### In Progress
*(note what you were working on when the session ended)*

### Next Up
- Newsletter signup placeholder (homepage section)
- Category pages (e.g. /explorer/cafes, /explorer/markets) — content to be added over time
- More Dubai Explorer + Connector content
- Third city (Lisbon is strong candidate)

### Decisions Made
- Framework: Astro v6 (static, fast, beginner-friendly, component-based)
- Styling: plain CSS with design tokens in src/styles/global.css — no Tailwind, no CSS-in-JS
- Mascot naming: "The Anchor" (not "The Settler") for settling/relocation guide
- Globe: CSS-only animated grid sphere for MVP; add new cities by editing the cities[] array in MapSection.astro
- Mascot images: SVG placeholders inline for now; swap with real PNGs in public/mascots/ when ready

---

## How to Resume After a Session Break

If starting a new Claude Code session, say:

> *"Please read CLAUDE.md and summarize the current state of the project, then let's continue from where we left off."*

That's it. Claude Code will read this file and pick up full context automatically.

---

*Landwell — a borderless community for people building life abroad* 🥔
