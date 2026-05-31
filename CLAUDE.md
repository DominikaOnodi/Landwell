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

- Framework: Astro v6 — static site, component-based, zero JS by default
- Styling: Plain CSS with design tokens in `src/styles/global.css` — no Tailwind
- Fonts: Cormorant Garamond (headings) + DM Sans (body) via Google Fonts
- Hosting: Netlify — auto-deploys from GitHub on every push
- Repo: GitHub (private), connected to Netlify
- Node: v22

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
- Dubai mascot hub pages built — /dubai/anchor, /dubai/explorer, /dubai/connector — session 5
- City routing fixed — Dubai city page portals now link to Dubai-specific mascot pages, not generic London ones — session 5
- MascotPage globe fixed — city pins now route to same mascot on the clicked city (e.g. London pin on Dubai Anchor → /anchor) — session 5
- Interactive D3 globe attempted — cobe and D3 approaches both rendered black; root cause is CDN/bundler environment issue, parked for now — session 5
- CSS globe restored with both London + Dubai pins — pure CSS, guaranteed to work everywhere — session 5
- PlaceCard redesigned — warm cream-dark background, no shadow, no pill tags (now dot-separated plain text), larger padding — session 5
- PartnerCard redesigned — same cream-dark treatment as PlaceCard for consistency — session 5
- Guide header redesigned — title smaller (max 30px), mascot smaller + softer, gradient fade from header colour into cream body — session 5
- Deployed to Netlify — site is live, auto-deploys on every GitHub push — session 5

### Completed (session 6)
- Globe locks on selected city — rotation stops permanently while a city is zoomed; clears when "← Back to globe" is clicked — session 6
- Newsletter wired to Netlify Forms — `data-netlify="true"` added; submissions appear in Netlify dashboard under Forms; AJAX submit so page doesn't reload — session 6
- Category cards redesigned from arch to full circles — semi-transparent white circles pick up zone-bg tint per mascot (sage/terracotta/mint) — session 6
- Connector page bg fixed — changed from `--cream-dark` to `--mint-pale` to match Dubai connector and the session 4 design decision — session 6

### Completed (session 7)
- Circle cards fixed properly — removed `align-items: center` from card wrapper (was causing oval/arch shape); now uses flex default stretch + `aspect-ratio: 1/1` for guaranteed perfect circles — session 7
- Circle cards darkened — background changed from semi-transparent white to `var(--cream-dark)` so they stand out against pale zone backgrounds — session 7
- Circle card spacing increased — grid gap raised from space-5 to space-8 across all mascot pages — session 7
- Dubai city page category cards converted to same circle style — HTML restructured with `.start-card__circle` + `.start-card__body`, CSS matches mascot pages — session 7
- Globe redesigned as Earth — blue ocean, green land, blue atmospheric rim glow, wider outer radiance; all from Canvas — session 7
- Night sky background added to globe section (mascot pages) — 240 twinkling stars, 4 subtle nebula patches, deep space `#05090f` background — session 7
- Night sky background applied to homepage globe section (MapSection) — same star field; text/card colours updated for dark background — session 7
- All session 7 changes committed and pushed; Netlify deployed — session 7

### In Progress
*(nothing — clean end to session 7)*

### Next Up — Priority Order

**Start of next session (confirmed):**
- Make category circle bubbles smaller — currently fill the full grid cell width, should be more compact
- Build the Connector section content — /connector has no guides yet; start with first category page (Events & Meetups or Language Exchange)

**Content to write:**
- Dubai Explorer guides: neighbourhoods, cafés/brunch, desert & outdoors
- Dubai Connector guides: expat communities, events & meetups
- London Connector content — /connector has no guides yet
- More London Explorer pages — parks, hidden gems

**Bigger features (future sessions):**
- Third city — Lisbon is the strongest candidate (D7 visa, NHR, enormous expat community, fits brand perfectly)
- Newsletter back-end — connect to Mailchimp or similar when ready
- Custom domain — point a real domain at the Netlify deployment
- SEO basics — add og:image, sitemap, meta descriptions per page
- Instagram feed or social proof section on homepage

### Decisions Made
- Framework: Astro v6 (static, fast, beginner-friendly, component-based)
- Styling: plain CSS with design tokens in src/styles/global.css — no Tailwind, no CSS-in-JS
- Mascot naming: "The Anchor" (not "The Settler") for settling/relocation guide
- Globe: CSS-only animated grid sphere is the stable choice for MVP; interactive D3/WebGL globe is aspirational — revisit once deployed site can be tested properly
- Mascot images: real PNGs in public/mascots/ — all loaded and working
- Routing: city-first then mascot (/dubai → /dubai/anchor); London mascot pages live at /anchor etc. not /london/anchor
- Cards: cream-dark background (#E3DBCE), no box-shadow, generous padding (space-8 / space-10)
- Hosting: Netlify, connected to GitHub, auto-deploy on push

---

## How to Resume After a Session Break

If starting a new Claude Code session, say:

> *"Please read CLAUDE.md and summarize the current state of the project, then let's continue from where we left off."*

That's it. Claude Code will read this file and pick up full context automatically.

---

*Landwell — a borderless community for people building life abroad* 🥔
