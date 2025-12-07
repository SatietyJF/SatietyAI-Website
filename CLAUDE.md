# SatietyAI Website - Project Context

> **This file is Claude Code's project memory. Read this first every session.**

## Project Overview

**What:** Hub website for SatietyAI (satietyai.io)
**Who:** AI beginners + Small business owners  
**Revenue:** Affiliate marketing, UGC services, Courses (future), Newsletter

**Deadline:** Launch-ready by December 7, 2025

## Two Audiences, One Site

The core design principle is **"Fish vs Learn to Fish"**:

1. **"Give me the fish"** → Tool recommendations with affiliate links (for busy business owners)
2. **"Teach me to fish"** → Project-based tutorials, learning paths (for AI learners)

Each department page serves BOTH audiences from the same content.

## Current Phase

**Phase:** Phase 1 - Foundation COMPLETE
**Session Goal:** Build section pages (Services, Newsletter, About, Learn, Business)
**Blockers:** None - ready to build pages

## Tech Stack

- **Framework:** Static HTML (chosen for speed to launch, zero config)
- **CSS:** Tailwind CSS via CDN
- **Hosting:** Cloudflare Pages
- **Email:** MailerLite (already configured with 5-email welcome sequence)
- **Analytics:** TBD (GA4 or Plausible)

## Brand Assets Status

| Asset | Status | Location |
|-------|--------|----------|
| Logo (dark/nav) | DONE | /assets/images/logo-dark.svg |
| Logo (light/footer) | DONE | /assets/images/logo-light.svg |
| Color Palette | DONE | See below (from Looka Brand Kit) |
| Fonts | DONE | Inter (Google Fonts) |

**Colors (from Looka Brand Kit):**
- Primary: `#3d84a8` (Teal blue)
- Secondary: `#591655` (Deep purple)
- Accent/CTA: `#E63946` (Bright red)
- Background: `#F8F9FA` (Off white)
- Text: `#1C1C1C` (Near black)

**Fonts:**
- Headings: Inter (600, 700 weights)
- Body: Inter (400, 500 weights)

## Site Structure

```
satietyai.io/
├── Homepage (hub with audience pathways)
├── /learn/ (AI Beginners)
│   ├── Getting Started
│   ├── Projects (placeholder)
│   └── Courses (waitlist)
├── /business/ (Small Business)
│   ├── Sales & Customer Service
│   ├── Marketing & Content
│   ├── Operations & Admin
│   ├── Finance & Accounting
│   ├── HR & Recruitment
│   └── Courses (waitlist)
├── /services/ (UGC Video)
│   ├── Overview + Pricing
│   └── Portfolio
├── /newsletter/
├── /about/
└── /legal/ (privacy, terms)
```

## Integration Details

### MailerLite

- **Account:** Configured ✅
- **Domain:** Authenticated ✅
- **Welcome Sequence:** 5 emails built ✅

**Form Tags to Use:**
- `website-signup` - General newsletter
- `learn-waitlist` - Beginner course interest
- `business-waitlist` - Business course interest

**Embed Code Location:** [ADD WHEN FORMS CREATED]

### Affiliate Links

| Program | Status | Link |
|---------|--------|------|
| Make.com | [APPROVED/PENDING] | [LINK] |
| Zapier | [APPROVED/PENDING] | [LINK] |
| Jasper.ai | [APPROVED/PENDING] | [LINK] |
| Copy.ai | [APPROVED/PENDING] | [LINK] |
| ClickBank | [APPROVED/PENDING] | [LINK] |
| Loom | PENDING (need site for Dec 7) | - |

## UGC Service Pricing

From planning docs - use these on services page:

| Package | Price | Includes |
|---------|-------|----------|
| Starter | $500-1,000 | 10 video package, 5-7 day delivery |
| Testing Suite | $1,500/mo | Unlimited variations, A/B ready |
| Full Service | $2,000/mo | Complete automation + strategy |

## Content Status

### Real Content (Use as-is)
- UGC pricing and descriptions
- Department AI applications (from planning docs)
- Affiliate program details

### Needs Writing
- Homepage tagline/value prop
- About page (founder story)

### Placeholder (Launch with "Coming Soon")
- Portfolio videos
- Tutorial projects
- Courses

## Key Files Reference

| File | Purpose |
|------|---------|
| `PROJECT_BRIEF.md` | Full specifications (this is the bible) |
| `TODO.md` | Current task list |
| `CHANGELOG.md` | What's been built |
| `CONTENT_STATUS.md` | Placeholder tracking |

## Design Decisions Log

Document choices here so we remember why:

| Date | Decision | Rationale |
|------|----------|-----------|
| 2025-11-30 | Static HTML over Astro/11ty | Faster to launch, zero config, ~20 pages manageable manually, can migrate later if needed |
| 2025-11-30 | Tailwind via CDN | No build step, instant setup, consistent design system |

## Known Issues

- [ ] [List any current issues]

## Next Session Priorities

1. Build Services page (UGC pricing - revenue generating, high priority)
2. Build Newsletter page (email capture)
3. Build About page (trust building)
4. Build Learn section pages
5. Build Business section pages
6. Add MailerLite form embeds

---

## Session Protocol

### Starting a Session

1. Read this file (CLAUDE.md)
2. Check TODO.md for current tasks
3. Review last CHANGELOG.md entry
4. Confirm session goal with Lewie

### Ending a Session

1. Update TODO.md (completed + new items)
2. Update CHANGELOG.md (what changed)
3. Update this file's "Next Session Priorities"
4. Commit with descriptive message
5. Summarize for Lewie

---

*Last Updated: 2025-12-01*
*Last Session: Opus - Logo integration fixed, brand colors updated to Looka Brand Kit values*
