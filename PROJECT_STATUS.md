# SatietyAI Website - Project Status & Handoff Document

> **FOR AI ASSISTANTS:** Read this file FIRST when continuing work on this project. It contains the complete context needed to pick up where the previous session left off.

---

## Quick Context

**What:** Marketing/hub website for SatietyAI (satietyai.io)
**Deadline:** December 7, 2025
**Tech Stack:** Static HTML + Tailwind CSS (via CDN) - no build step required
**Hosting:** Cloudflare Pages

---

## Project Goals

### Primary Purpose
Build a professional website that serves TWO audiences from the same content:

1. **AI Beginners** - Want to learn AI through hands-on projects
2. **Small Business Owners** - Want AI tool recommendations for their departments

### Revenue Model (What the site supports)
| Revenue Stream | How Site Supports It |
|----------------|---------------------|
| Affiliate Marketing | Tool recommendation pages with affiliate links |
| UGC Video Services | Service page with pricing, portfolio, contact |
| Course Sales | "Coming Soon" waitlist pages |
| Newsletter | Email capture forms throughout site |

### Core Design Principle: "Fish vs Learn to Fish"
Every department page should offer BOTH:
- **"Give me the fish"** → Direct tool recommendations (affiliate links)
- **"Teach me to fish"** → Tutorials and learning resources

---

## Site Architecture

```
src/
├── index.html              ← Homepage (BUILT)
├── learn/
│   ├── index.html          ← Learn overview
│   ├── getting-started.html
│   ├── projects.html       ← Placeholder grid
│   └── courses.html        ← Waitlist page
├── business/
│   ├── index.html          ← Business overview
│   ├── sales.html          ← Department page template
│   ├── marketing.html
│   ├── operations.html
│   ├── finance.html
│   ├── hr.html
│   └── courses.html        ← Waitlist page
├── services/
│   ├── index.html          ← UGC pricing page
│   └── portfolio.html      ← Placeholder
├── newsletter/
│   └── index.html          ← Dedicated signup
├── about/
│   └── index.html
├── legal/
│   ├── privacy.html
│   └── terms.html
└── assets/
    ├── css/
    ├── js/
    └── images/
        └── logo.png        ← Brand logo
```

---

## Current Status

### What's Been Built
| Item | Status | Notes |
|------|--------|-------|
| Project structure | DONE | All folders created |
| Homepage (index.html) | DONE | Full layout with Looka brand colors |
| Navigation component | DONE | Desktop + mobile menu, SVG logo integrated |
| Footer component | DONE | Full footer with all links, white SVG logo |
| Tailwind config | DONE | Brand colors from Looka Brand Kit |
| Logo SVGs | DONE | logo-dark.svg (nav), logo-light.svg (footer) |
| PROJECT_STATUS.md | DONE | Handoff document for future sessions |

### What's NOT Built Yet
- All section pages (learn/, business/, services/, etc.)
- MailerLite form integration (have account, need embed codes)
- Affiliate links (pending approvals)
- About page content
- Legal pages

### Placeholders in Current Build
| Location | Placeholder | Needs |
|----------|-------------|-------|
| Homepage hero | `[Your AI Journey Starts Here]` | Tagline from Lewie |
| Newsletter forms | HTML form | MailerLite embed code |
| Social links | `href="#"` | Actual social URLs |

---

## Brand Assets

### Logo
- **Dark version (nav):** `src/assets/images/logo-dark.svg` - Black swirl, purple text
- **Light version (footer):** `src/assets/images/logo-light.svg` - All white
- **Design:** Circular wave/swirl symbol + "SATIETY AI" text + "AI SATISFACTION" tagline
- **Source:** Looka Brand Kit (looka.com/brandkit/232073523)

### Color Palette (FINALIZED - from Looka Brand Kit)

```javascript
// In Tailwind config (src/index.html <script>)
colors: {
    primary: '#3d84a8',      // Teal blue (from Looka)
    secondary: '#591655',    // Deep purple (from Looka)
    accent: '#E63946',       // Bright red (CTA buttons)
    teal: '#3d84a8',         // Same as primary
    dark: '#1C1C1C',         // Text color
    light: '#F8F9FA',        // Background
}
```

**Color usage:**
- `primary` / `teal` - Nav links, buttons, Learn section accents
- `secondary` - Business section accents, hover states, logo text
- `accent` - Subscribe/CTA buttons (stands out)

### Typography
- **Current:** Inter (Google Fonts)
- **Status:** Approved by default, can change if Lewie prefers

---

## Technical Details

### How the Site Works
1. **No build step** - Open HTML files directly in browser to preview
2. **Tailwind via CDN** - Colors configured in `<script>` tag in each HTML file
3. **Static hosting** - Upload `src/` folder contents to Cloudflare Pages

### File Structure Pattern
Each HTML page includes:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta, Tailwind CDN, custom colors config, fonts -->
</head>
<body>
    <!-- Nav (copy from index.html) -->
    <!-- Page content -->
    <!-- Footer (copy from index.html) -->
    <!-- Mobile menu script -->
</body>
</html>
```

### To Update Colors Site-Wide
1. Define final hex values
2. Update the `tailwind.config` script block in EACH HTML file
3. Or: Extract to a shared `assets/js/tailwind-config.js` file

### Key CSS Classes Used
- `bg-primary`, `text-primary`, `hover:bg-primary` - Main brand color
- `bg-secondary` - Secondary brand color
- `bg-accent` - CTA buttons
- `bg-dark`, `text-dark` - Dark text/backgrounds
- `bg-light` - Light backgrounds

---

## Integration Notes

### MailerLite
- **Account:** Configured and authenticated
- **Welcome sequence:** 5 emails already built
- **Form tags to use:**
  - `website-signup` - General newsletter
  - `learn-waitlist` - Beginner course interest
  - `business-waitlist` - Business course interest
- **TO DO:** Get embed code from MailerLite dashboard, replace placeholder `<form>` elements

### Affiliate Programs
| Program | Status | Commission |
|---------|--------|------------|
| Make.com | PENDING | Recurring |
| Zapier | PENDING | 30% recurring |
| Jasper.ai | PENDING | 30% recurring |
| Copy.ai | PENDING | 30% recurring |
| ClickBank | PENDING | 50-75% |

### UGC Service Pricing (Use on services page)
| Package | Price | Details |
|---------|-------|---------|
| Starter | $500-1,000 | 10 videos, 5-7 day delivery |
| Testing Suite | $1,500/mo | Unlimited variations, A/B ready |
| Full Service | $2,000/mo | Complete automation + strategy |

---

## For Future Sessions

### Immediate Next Steps
1. Finalize color palette with Lewie
2. Update homepage with final colors
3. Build core pages: About, Newsletter, Services
4. Build Learn section (4 pages)
5. Build Business section (7 pages)
6. Add MailerLite embeds
7. Test and deploy

### Page Build Priority
1. **Homepage** - DONE (needs color update)
2. **Services** - Revenue generating, high priority
3. **Newsletter** - Email capture
4. **About** - Trust building
5. **Learn section** - Audience path
6. **Business section** - Audience path (can template one, copy for others)
7. **Legal pages** - Required for launch

### Content Still Needed from Lewie
- [ ] Homepage tagline/value proposition
- [ ] About page founder story
- [ ] Final color hex codes
- [ ] Social media URLs (YouTube, LinkedIn, Instagram)
- [ ] MailerLite form embed codes

---

## Reference Documents

| File | Purpose |
|------|---------|
| `CLAUDE.md` | Session-by-session project memory |
| `TODO.md` | Active task tracking |
| `CHANGELOG.md` | What's been built/changed |
| `docs/satietyai-website-project-brief.md` | Full specifications |

---

## Commands for Development

```bash
# Preview site locally (just open in browser)
# No server needed - double-click src/index.html

# Or use Python simple server if needed:
cd src && python -m http.server 8000
# Then visit http://localhost:8000

# Deploy to Cloudflare Pages:
# Connect GitHub repo, set build output to "src/"
```

---

*Last Updated: December 1, 2025*
*Last Session: Opus - Logo SVGs fixed (viewBox issue), brand colors updated to Looka Brand Kit values (#3d84a8 teal, #591655 purple)*
