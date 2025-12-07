# SatietyAI Website Project Brief
## For Claude Code CLI Implementation

**Project:** satietyai.io Website Build
**Created:** November 30, 2025
**Status:** Planning Complete - Ready for Implementation

---

## Project Overview

### Mission
Build a professional hub website for SatietyAI that serves two primary audiences while supporting four revenue pillars.

### Target Audiences

1. **AI Beginners** - Want to learn AI through hands-on projects, build practical skills
2. **Small Business Owners** - Want department-specific AI integration, save time, implement tools

### Revenue Pillars the Site Must Support

| Pillar | Website Function | Priority |
|--------|------------------|----------|
| Affiliate Marketing | Tool recommendations with affiliate links | HIGH |
| UGC Video Services | Service pages, portfolio, inquiry forms | HIGH |
| Course Sales | Coming soon pages, waitlists | MEDIUM |
| Newsletter | Email capture throughout site | HIGH |

---

## Site Architecture

```
satietyai.io/
│
├── index.html (Homepage Hub)
│
├── /learn/ (AI Beginners Section)
│   ├── index.html (Learning overview)
│   ├── getting-started.html
│   ├── projects.html (placeholder for tutorials)
│   └── courses.html (coming soon + waitlist)
│
├── /business/ (Small Business Section)
│   ├── index.html (Business overview)
│   ├── sales.html (Sales & Customer Service dept)
│   ├── marketing.html (Marketing & Content dept)
│   ├── operations.html (Operations & Admin dept)
│   ├── finance.html (Finance & Accounting dept)
│   ├── hr.html (HR & Recruitment dept)
│   └── courses.html (coming soon + waitlist)
│
├── /services/ (UGC Video Services)
│   ├── index.html (Service overview + pricing)
│   └── portfolio.html (Video examples)
│
├── /newsletter/ (Dedicated signup page)
│   └── index.html
│
├── /about/
│   └── index.html
│
├── /legal/
│   ├── privacy.html
│   └── terms.html
│
└── /assets/
    ├── /css/
    ├── /js/
    ├── /images/
    └── /fonts/
```

---

## Page Specifications

### Homepage (index.html)

**Purpose:** Hub entry point with clear audience pathways

**Sections (in order):**

1. **Hero Section**
   - Logo (placeholder: `[LOGO]`)
   - Tagline: `[PLACEHOLDER: Main value proposition]`
   - Newsletter signup form (MailerLite embed)
   - Brief intro text

2. **Audience Pathway Section**
   - Two prominent cards/boxes:
     - **"New to AI?"** → Links to /learn/
     - **"Ready to Implement AI in Your Business?"** → Links to /business/
   - Clear visual distinction between paths

3. **What We Offer (Brief)**
   - 3-4 cards showing: Learning Resources, Business Solutions, UGC Services, Newsletter
   - Each links to relevant section

4. **Social Proof (Placeholder)**
   - Placeholder for testimonials/logos when available
   - Can show "As featured in..." or stats

5. **Footer**
   - Navigation links
   - Social media links (YouTube, LinkedIn, Instagram)
   - Newsletter signup (secondary)
   - Legal links (Privacy, Terms)

---

### Learn Section (/learn/)

**Overview Page (/learn/index.html)**
- Introduction to learning path
- What you'll learn
- Cards linking to: Getting Started, Projects, Courses

**Getting Started (/learn/getting-started.html)**
- Beginner-friendly intro to AI
- First steps to take
- Tool recommendations (affiliate links)
- Newsletter CTA

**Projects (/learn/projects.html)**
- Header explaining project-based learning
- "Coming Soon" grid of project placeholders
- Each placeholder shows: Project name, difficulty level, what you'll build
- Newsletter CTA: "Get notified when new projects drop"

**Courses (/learn/courses.html)**
- "Courses Coming Soon" announcement
- Course previews (placeholders):
  - "AI Fundamentals" - Hands-on introduction
  - "Build Your First Automation" - Project course
- Waitlist signup form (MailerLite)
- "In the meantime, join our newsletter" CTA

---

### Business Section (/business/)

**Overview Page (/business/index.html)**
- Value prop for small business owners
- Department grid with links to each department page
- "Don't know where to start?" → links to Sales (recommended first)

**Department Pages Template (sales.html, marketing.html, etc.)**

Each department page follows this dual-serve structure:

1. **Header**
   - Department name
   - "AI for [Department]: Save Time, Work Smarter"

2. **The Problem**
   - Pain points in this department
   - What's possible with AI

3. **"Get the Solution" Section (Affiliate Path)**
   - Heading: "Recommended Tools"
   - Subheading: "These are the tools I use and recommend"
   - Tool cards with:
     - Tool name
     - Brief description (1-2 sentences)
     - "Try it →" button (affiliate link)
   - Placeholder for 3-5 tools per department

4. **"Learn to Build It" Section (Learning Path)**
   - Heading: "Learn to Implement This Yourself"
   - Project/tutorial placeholders
   - Links to relevant YouTube videos (when available)
   - Newsletter CTA: "Get step-by-step tutorials in your inbox"

5. **Courses Section**
   - "Master [Department] AI - Course Coming Soon"
   - Waitlist signup

**Business Courses (/business/courses.html)**
- Same structure as /learn/courses.html but business-focused
- Course previews:
  - "AI for [Department] - 30 Day Implementation" (mini-course)
  - "Complete AI Business Transformation" (flagship)
- Waitlist signup

---

### Services Section (/services/)

**Overview Page (/services/index.html)**

1. **Hero**
   - "UGC Videos That Convert"
   - Subheadline about AI-powered, authentic content

2. **The Problem**
   - Traditional UGC is expensive ($500-2000/video)
   - Takes 5-14 days
   - Hard to test variations

3. **The Solution**
   - AI-powered UGC video generation
   - Authentic, not "AI-looking"
   - Multiple variations for testing

4. **Pricing Packages**
   - **Starter Package**: $500-1000 for 10 videos
     - Perfect for testing
     - Multiple variations
     - 5-7 day delivery
   - **Content Testing Suite**: $1,500/month
     - Unlimited video variations
     - A/B testing ready
     - Priority delivery
   - **Full-Service Automation**: $2,000/month
     - Complete social media automation
     - Strategy included
     - Dedicated support

5. **Portfolio Preview**
   - "See Our Work" section
   - Placeholder grid for video thumbnails
   - "View Full Portfolio →" link

6. **CTA Section**
   - "Ready to Get Started?"
   - Contact form or Calendly embed
   - Or: "Have questions? Email [email]"

**Portfolio Page (/services/portfolio.html)**
- Grid of video examples
- Placeholder state: "Portfolio in Development"
- Message: "Our first client projects are in production. Check back soon or contact us to discuss your project."
- Inquiry CTA

---

### Newsletter Page (/newsletter/)

**Dedicated signup landing page**

1. **Hero**
   - "AI Tips That Actually Work"
   - "Weekly insights for AI learners and implementers"

2. **What You Get**
   - Weekly AI tips and tutorials
   - Tool recommendations and deals
   - First access to courses and resources
   - No spam, unsubscribe anytime

3. **Signup Form**
   - MailerLite embed
   - Name + Email fields
   - Submit button

4. **Social Proof**
   - Subscriber count (when available)
   - Or: "Join [X] others learning AI"

---

### About Page (/about/)

1. **Who We Are**
   - The SatietyAI story
   - Mission statement
   - Placeholder: `[FOUNDER STORY TO BE WRITTEN]`

2. **What We Believe**
   - Education-first approach
   - Practical, not theoretical
   - AI should save time, not create complexity

3. **Connect**
   - Social links
   - Newsletter CTA
   - Contact info

---

### Legal Pages (/legal/)

**Privacy Policy (/legal/privacy.html)**
- Standard privacy policy covering:
  - What data we collect (email for newsletter)
  - How we use it
  - Third-party tools (MailerLite)
  - Affiliate disclosure
  - Cookie policy
  - Contact for questions

**Terms of Service (/legal/terms.html)**
- Standard terms for:
  - Website use
  - Service agreements (for UGC services)
  - Disclaimer

---

## Design Specifications

### Brand Elements

**Logo**
- Placeholder: `[LOGO - TO BE PROVIDED]`
- Format needed: SVG preferred, PNG fallback
- Sizes needed: Full logo, icon-only version

**Color Palette**
- Placeholder: `[TO BE DERIVED FROM LOGO]`
- Structure needed:
  - Primary color (brand main)
  - Secondary color (accent)
  - Background (light)
  - Text (dark)
  - Success/CTA color

**Typography**
- Headings: `[TO BE DECIDED - suggest: Inter, Poppins, or Montserrat]`
- Body: `[TO BE DECIDED - suggest: Inter or system fonts]`
- Fallback: system-ui, -apple-system, sans-serif

### Design Principles

1. **Professional but approachable** - Not corporate, not casual
2. **Clean and fast** - Minimal decoration, focus on content
3. **Mobile-first** - Instagram traffic will be mobile
4. **Clear hierarchy** - Easy to scan, obvious CTAs
5. **Consistent** - Same patterns repeated across pages

### Component Patterns

**Cards**
- Used for: Audience pathways, department links, tool recommendations, course previews
- Structure: Optional icon, title, brief description, link/button

**CTAs (Call to Action)**
- Primary: Filled button, primary color
- Secondary: Outlined button
- Newsletter forms: Inline horizontal on desktop, stacked on mobile

**Navigation**
- Desktop: Horizontal nav with dropdown for Learn/Business sections
- Mobile: Hamburger menu with full-screen overlay

**Footer**
- Consistent across all pages
- Columns: Quick links, Services, Connect, Newsletter signup
- Bottom: Copyright, legal links

---

## Technical Specifications

### Stack Recommendation

**Option A: Static HTML/CSS/JS (Simplest)**
- Pure HTML pages
- CSS (custom or Tailwind)
- Vanilla JS for interactions
- Best for: Fast build, easy hosting

**Option B: Static Site Generator (Recommended)**
- Astro or 11ty
- Component-based development
- Markdown for content pages (easy updates)
- Best for: Maintainability, future content additions

### Hosting

**Recommended: Cloudflare Pages**
- Free tier sufficient
- Fast global CDN
- Easy deployment from Git
- Already have Cloudflare integration

**Alternative: Netlify or Vercel**
- Also free tier
- Similar capabilities

### Integrations

**Email (MailerLite)**
- Embed forms using MailerLite's embed code
- Forms needed on:
  - Homepage (hero)
  - Newsletter page
  - Course waitlist pages
  - Footer (all pages)
- Tags to use:
  - `website-signup` (general)
  - `learn-waitlist` (beginner courses)
  - `business-waitlist` (business courses)

**Analytics**
- Google Analytics 4 or Plausible (privacy-friendly)
- Track: Page views, form submissions, outbound link clicks

**Affiliate Links**
- Structure: Use descriptive slugs or UTM parameters
- Example: `make.com/?ref=satietyai` or track via Pretty Links if needed

---

## Content Placeholders

These items need to be created/provided before or during build:

### Must Have for Launch

| Item | Status | Notes |
|------|--------|-------|
| Logo | IN PROGRESS | Lewie finalizing today |
| Homepage value prop | NEEDED | 1-2 sentence tagline |
| About page copy | NEEDED | Founder story, mission |
| UGC Services descriptions | NEEDED | Package details exist in planning docs |
| Privacy policy | NEEDED | Template can be adapted |
| Terms of service | NEEDED | Template can be adapted |

### Can Launch with Placeholders

| Item | Placeholder Text |
|------|------------------|
| Portfolio videos | "Portfolio in Development - First projects in production" |
| Department tool recommendations | "Tool recommendations coming soon" (or add 1-2 per dept) |
| Learning projects | "Projects coming soon - Join newsletter for updates" |
| Courses | "Courses launching 2026 - Join waitlist" |
| Testimonials | Section can be hidden initially |

---

## Affiliate Links Reference

From planning documents, priority affiliate programs:

| Tool | Commission | Department Focus |
|------|------------|------------------|
| Make.com | Recurring | All departments |
| Zapier | 30% recurring | All departments |
| Jasper.ai | 30% recurring | Marketing, Content |
| Copy.ai | 30% recurring | Marketing, Content |
| HubSpot | Varies | Sales, CRM |
| Pipedrive | Varies | Sales, CRM |
| ClickBank courses | 50-75% | Learning section |

**Note:** Affiliate links to be added as accounts are approved. Placeholder buttons can link to tool homepages initially.

---

## Launch Checklist

### Pre-Launch (Before Dec 7)

- [ ] Logo finalized and exported (SVG + PNG)
- [ ] Color palette defined
- [ ] Homepage copy written
- [ ] About page copy written
- [ ] Privacy policy created
- [ ] Terms of service created
- [ ] MailerLite forms configured with correct tags
- [ ] All pages built and linked
- [ ] Mobile responsiveness tested
- [ ] Forms tested (submissions reach MailerLite)
- [ ] Affiliate links added where approved
- [ ] Analytics installed
- [ ] DNS configured (if not already)
- [ ] SSL certificate active

### Post-Launch (Ongoing)

- [ ] Add portfolio pieces as created
- [ ] Fill in department tool recommendations
- [ ] Add YouTube video embeds as published
- [ ] Build out project tutorials
- [ ] Update course information as developed

---

# PART 2: Claude Code CLI Project Management

## Project Structure for Claude Code

When starting this project in Claude Code CLI, use the following structure for organization, memory, and tracking.

### Directory Structure

```
satietyai-website/
│
├── CLAUDE.md                 # Project memory/context file (CRITICAL)
├── TODO.md                   # Active task tracking
├── CHANGELOG.md              # What's been built/changed
│
├── docs/                     # Project documentation
│   ├── PROJECT_BRIEF.md      # This document (reference)
│   ├── DESIGN_DECISIONS.md   # Why we built things certain ways
│   ├── CONTENT_STATUS.md     # Track placeholder vs real content
│   └── INTEGRATIONS.md       # MailerLite setup, analytics, etc.
│
├── src/                      # Source code
│   ├── index.html
│   ├── learn/
│   ├── business/
│   ├── services/
│   ├── newsletter/
│   ├── about/
│   ├── legal/
│   └── assets/
│       ├── css/
│       ├── js/
│       └── images/
│
├── dist/                     # Built/deployable files (if using build step)
│
└── .github/                  # GitHub Actions for deployment (optional)
    └── workflows/
```

---

## CLAUDE.md Template

Create this file at project root. Claude Code CLI will reference it for context.

```markdown
# SatietyAI Website - Project Context

## Project Overview
Building satietyai.io - a hub website serving AI beginners and small business owners.
Four revenue pillars: Affiliate marketing, UGC services, Course sales, Newsletter.

## Current Phase
[UPDATE AS YOU PROGRESS]
- Phase: Initial Build
- Priority: Launch-ready site by Dec 7, 2025
- Focus: Core pages, email capture, UGC services

## Tech Stack
- [TO BE DECIDED: Static HTML or Astro/11ty]
- CSS: [Tailwind / Custom]
- Hosting: Cloudflare Pages
- Email: MailerLite
- Analytics: [GA4 / Plausible]

## Key Files
- PROJECT_BRIEF.md: Full specifications
- TODO.md: Current tasks
- CONTENT_STATUS.md: What's placeholder vs real

## Brand Assets
- Logo: [STATUS]
- Colors: [PRIMARY] [SECONDARY] [ACCENT]
- Fonts: [HEADING FONT] / [BODY FONT]

## Integration Details
### MailerLite
- Account: [configured]
- Forms:
  - Homepage signup: [FORM_ID]
  - Newsletter page: [FORM_ID]
  - Course waitlist (learn): [FORM_ID]
  - Course waitlist (business): [FORM_ID]

### Affiliate Links
- Make.com: [LINK or PENDING]
- Zapier: [LINK or PENDING]
- [Add as approved]

## Design Decisions Log
[Document why certain choices were made]
- [Date]: Chose [X] over [Y] because...

## Known Issues / Blockers
- [List any current blockers]

## Next Session Priorities
[Update at end of each session]
1. 
2. 
3. 
```

---

## TODO.md Template

```markdown
# SatietyAI Website - Task Tracker

## Currently Working On
- [ ] [Active task]

## Up Next (Priority Order)
1. [ ] 
2. [ ] 
3. [ ] 

## Backlog

### Infrastructure
- [ ] Initialize project structure
- [ ] Set up CSS framework/approach
- [ ] Configure build process (if using SSG)
- [ ] Set up Cloudflare Pages deployment

### Pages - Core (Must Have for Launch)
- [ ] Homepage
- [ ] About page
- [ ] Newsletter signup page
- [ ] Services overview
- [ ] Privacy policy
- [ ] Terms of service

### Pages - Learn Section
- [ ] Learn overview
- [ ] Getting started
- [ ] Projects (placeholder)
- [ ] Courses (waitlist)

### Pages - Business Section
- [ ] Business overview
- [ ] Sales department
- [ ] Marketing department
- [ ] Operations department
- [ ] Finance department
- [ ] HR department
- [ ] Courses (waitlist)

### Pages - Services
- [ ] Services/pricing page
- [ ] Portfolio page

### Integrations
- [ ] MailerLite forms embedded
- [ ] Analytics installed
- [ ] Affiliate links added

### Content
- [ ] Homepage copy
- [ ] About page copy
- [ ] Service descriptions
- [ ] Legal pages

### Design
- [ ] Logo integration
- [ ] Color palette implementation
- [ ] Typography setup
- [ ] Mobile responsiveness
- [ ] Component patterns (cards, buttons, forms)

## Completed
- [x] Project brief created
- [x] [Add completed items with dates]

## Blocked / Waiting
- [ ] [Item]: Waiting on [what]
```

---

## CHANGELOG.md Template

```markdown
# SatietyAI Website - Changelog

## [Unreleased]
### Added
- 

### Changed
- 

### Fixed
- 

---

## [0.1.0] - YYYY-MM-DD (Initial Launch)
### Added
- Initial site structure
- Core pages: Home, About, Services, Newsletter
- Learn section with placeholder content
- Business section with department pages
- MailerLite integration
- Privacy and Terms pages
```

---

## CONTENT_STATUS.md Template

```markdown
# Content Status Tracker

## Real Content (Complete)
| Page | Section | Status | Notes |
|------|---------|--------|-------|
| Services | Pricing | ✅ | From planning docs |
| | | | |

## Placeholder Content (Needs Creation)
| Page | Section | Placeholder Text | Priority |
|------|---------|------------------|----------|
| Homepage | Hero tagline | [NEEDS COPY] | HIGH |
| About | Founder story | [NEEDS COPY] | HIGH |
| Portfolio | Video examples | "In Development" | MEDIUM |
| Learn/Projects | Tutorial list | "Coming Soon" | LOW |
| All Depts | Tool recommendations | "Coming Soon" or basic list | MEDIUM |

## Content Creation Queue
1. Homepage value proposition
2. About page founder story
3. Department tool recommendations (start with Sales)
4. Portfolio pieces (as UGC projects complete)
```

---

## Modular Development Approach

### Phase 1: Foundation (Sessions 1-2)

**Goal:** Project setup, base layout, one complete page

1. Initialize project structure
2. Set up CSS approach (recommend Tailwind for speed)
3. Create base layout template (header, footer, nav)
4. Build homepage completely
5. Test MailerLite integration

**Checkpoint:** Homepage live and functional

### Phase 2: Core Pages (Sessions 3-4)

**Goal:** All "must have" pages for launch

1. About page
2. Newsletter page
3. Services page (with pricing)
4. Legal pages (privacy, terms)

**Checkpoint:** Core site navigable and professional

### Phase 3: Learn Section (Session 5)

**Goal:** Beginner audience pathway complete

1. Learn overview
2. Getting started page
3. Projects page (placeholders)
4. Courses page (waitlist)

**Checkpoint:** Learn section complete

### Phase 4: Business Section (Sessions 6-7)

**Goal:** Business audience pathway complete

1. Business overview
2. Department pages (use template, build 1-2 fully, rest placeholder)
3. Business courses page (waitlist)

**Checkpoint:** Business section complete

### Phase 5: Polish & Launch (Session 8)

**Goal:** Launch-ready

1. Mobile testing and fixes
2. Cross-browser testing
3. Analytics verification
4. Final content review
5. Deploy to production

**Checkpoint:** Site live at satietyai.io

---

## Session Start Protocol

At the beginning of each Claude Code session:

1. **Read CLAUDE.md** for project context
2. **Check TODO.md** for current priorities
3. **Review last CHANGELOG.md entry** for what was done
4. **Confirm current phase** and goals

### Prompt Template for Session Start

```
I'm continuing work on the SatietyAI website. 

Please read:
- CLAUDE.md (project context)
- TODO.md (current tasks)
- CHANGELOG.md (recent work)

My focus this session: [SPECIFIC GOAL]

Current blockers or notes: [ANY CONTEXT]
```

---

## Session End Protocol

At the end of each Claude Code session:

1. **Update TODO.md** - Mark completed, add new items
2. **Update CHANGELOG.md** - What was built/changed
3. **Update CLAUDE.md** - Next session priorities, any new context
4. **Commit changes** with descriptive message

### Prompt Template for Session End

```
Let's wrap up this session. Please:

1. Update TODO.md with what we completed and what's next
2. Add today's changes to CHANGELOG.md
3. Update CLAUDE.md "Next Session Priorities" section
4. Summarize what we accomplished and what to tackle next time
```

---

## Handling Blockers

When you hit a blocker (missing content, design decision needed, etc.):

1. **Document it** in TODO.md under "Blocked / Waiting"
2. **Note what's needed** specifically
3. **Move on** to non-blocked tasks
4. **Flag for Lewie** in session summary

### Example Blocker Documentation

```markdown
## Blocked / Waiting
- [ ] Homepage hero section: Waiting on tagline copy from Lewie
- [ ] Logo integration: Waiting on final logo files (SVG + PNG)
- [ ] Sales page tools: Need to confirm which affiliates are approved
```

---

## Quality Checkpoints

### After Each Page Build

- [ ] Page loads without errors
- [ ] All links work (internal and external)
- [ ] Forms submit correctly (test with MailerLite)
- [ ] Responsive on mobile (320px minimum)
- [ ] Content is readable and hierarchy is clear
- [ ] Consistent with other pages (nav, footer, styling)

### Before Launch

- [ ] All pages complete and linked
- [ ] Forms working and tagged correctly
- [ ] Analytics tracking
- [ ] Legal pages present
- [ ] Mobile experience is good
- [ ] Load time acceptable (<3s)
- [ ] No broken images or missing assets
- [ ] Affiliate disclosure present where needed

---

## Recovery Procedures

### If Something Breaks

1. Check git log for recent changes
2. Identify what changed
3. Revert if necessary: `git revert [commit]`
4. Document in CHANGELOG.md what happened

### If Context is Lost

1. Read CLAUDE.md thoroughly
2. Read PROJECT_BRIEF.md for full specifications
3. Check TODO.md for where we left off
4. Review recent git commits

### If Unsure About a Decision

1. Check DESIGN_DECISIONS.md for precedent
2. Check PROJECT_BRIEF.md for requirements
3. If still unclear, make a reasonable choice and document it
4. Flag for Lewie's review

---

# Quick Reference

## File Purposes

| File | Purpose | Update Frequency |
|------|---------|------------------|
| CLAUDE.md | Project memory, current state | Every session |
| TODO.md | Task tracking | Every session |
| CHANGELOG.md | What's changed | Every session |
| PROJECT_BRIEF.md | Full specifications | Rarely (reference) |
| DESIGN_DECISIONS.md | Why we built things | As decisions made |
| CONTENT_STATUS.md | Placeholder tracking | As content added |

## Key Commands

```bash
# Start dev server (if using Astro)
npm run dev

# Build for production
npm run build

# Deploy to Cloudflare Pages
# (Usually automatic via git push if configured)
```

## Important Links

- Domain registrar: Namecheap
- Email: MailerLite dashboard
- Hosting: Cloudflare Pages dashboard
- Analytics: [GA4 / Plausible dashboard]

---

*This document is the single source of truth for the SatietyAI website project. Keep it updated and reference it often.*
