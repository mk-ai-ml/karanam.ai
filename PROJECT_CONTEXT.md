# karanam.ai — Personal Professional Website
## Project Context for Cowork

---

## Owner
**Manohar Karanam** | Strategic AI, ML & Data Science Leader
- Email: manohar.karanam18@gmail.com
- LinkedIn: linkedin.com/in/manohar-karanam
- Location: Vadodara, Gujarat, India
- GitHub: mk-ai-ml
- Hugging Face: mk-ai-ml

---

## Project Goal
Build and maintain a clean, professional personal website to showcase Manohar's work and thought leadership to his professional network (individuals + LinkedIn). The site will evolve regularly — new projects, articles, and case studies will be added over time.

---

## Domain
- **Working assumption:** `karanam.ai` (not yet purchased)
- Other shortlisted options: `manoharai.com`, `mkaranam.com`
- Decision pending — domain not yet bought

---

## Tech Stack (Agreed)
| Layer | Choice |
|---|---|
| Framework | **Astro** (file-based, fast, great for portfolios) |
| Hosting | **GitHub Pages / Netlify** (free, auto-deploy on git push) |
| Content updates | Edit `.astro` or `.md` files |
| Future blog | Astro's built-in MDX support |
| Node.js work | Claude/Cowork handles all of this |

> **Note:** Manohar is comfortable with a Git + Netlify workflow. He will handle content edits; Claude/Cowork handles all code.

---

## Current State
- ✅ **Landing page built** — single `index.html` file (pre-Astro prototype for review)
- ✅ File location: `outputs/index.html`
- ✅ Design approved (with minor tweaks)
- ⬜ Domain not yet purchased
- ⬜ GitHub repo not yet created
- ⬜ Netlify not yet set up
- ⬜ Astro project not yet scaffolded
- ⬜ Projects section intentionally removed — to be added when content is ready

---

## Design Decisions (Locked)

### Theme
- **Tone:** Sophisticated but approachable — warm gravitas (not intimidating)
- **Mode:** Light theme — warm parchment/linen base
- **Palette:**
  - Background: `#faf7f2` (warm linen)
  - Surface: `#f3ede3`
  - Accent/Gold: `#b5813a` (earthy amber)
  - Text: `#2c2416` (deep espresso brown)
  - Muted text: `#6b5c42`
- **Fonts:** Playfair Display (headings, serif, editorial gravitas) + DM Sans (body, clean) + DM Mono (labels/tags)
- **Hero:** Warm gradient (linen → soft peach), decorative grid background on right panel

### Layout & Sections (in order)
1. **Nav** — Fixed, `karanam.ai` logo left, section links right
2. **Hero** — Name, title, IIM/BITS credential line, positioning blurb, 4 impact stats grid, 2 CTAs
3. **About** — Sticky sidebar with heading + geo tags (India/UK/AU/DK), 3-para story right
4. **Expertise** — 6 cards: GenAI & RAG, AI Strategy & 0→1, AI Monetisation, Team Leadership, MLOps, BFSI/CPG/Manufacturing
5. **Work Timeline** — Vertical timeline, gold left border, 6 roles (see below)
6. **Recognition** — 6 awards in grid
7. **Contact** — Centered, email + LinkedIn CTAs
8. **Footer** — Warm surface bg, copyright + tagline

### Sections Intentionally Excluded
- **Projects section removed** — will be re-added when Manohar has solid content ready (e.g., RAG playbook, case studies, research)

---

## Work Timeline Content (6 Roles)

| Period | Role | Company |
|---|---|---|
| Nov 2024 – Present | Senior Data Science Manager | PGP Glass Pvt. Ltd. |
| Oct 2023 – Oct 2024 | Co-Founder & Partner | The AI Corp |
| Jan 2022 – Oct 2023 | Data Science Manager | Paytm |
| Dec 2019 – Jan 2022 | Senior Data Scientist (Sr. Architect) | Mindtree — Unilever APAC |
| Mar 2015 – Nov 2018 | Senior Software Engineer — Analytics CoE | Danske IT |
| Jul 2007 – Feb 2015 | Technology Analyst | Infosys Ltd. (RBS, AMP, NAB) |

---

## Key Impact Numbers (used in Hero stats & timeline pills)
- 17+ years experience
- 70+ enterprise AI use cases delivered
- 4× fraud detection uplift (Danske)
- 2.5× sales conversion improvement (Unilever)
- ₹1 Cr/month → breakeven in 2 quarters (Paytm)
- 20–40% churn reduction (Paytm)
- 1.5–2× recommendation uplift (Unilever)
- 10–20% customer growth (Unilever)
- 1–2% manufacturing efficiency gain (PGP Glass)

---

## Pending Decisions / Next Steps

### Immediate
1. **Domain purchase** — Manohar to finalise name and buy (Namecheap or Cloudflare Registrar recommended)
2. **Saama research content** — Manohar to upload folder; Claude to assess, strip company references, and determine if it belongs on the site
3. **GitHub repo setup** — Create `karanam-ai` repo, push `index.html`
4. **Netlify deployment** — Connect repo, configure auto-deploy
5. **Astro migration** — Scaffold proper Astro project for maintainability

### Future Additions
- Projects section (when content is ready)
- Blog / Articles section (Astro MDX)
- Case studies (anonymised from past work)
- Speaking / Advisory section (if relevant)

---

## Important Rules for This Project
- **Never expose private projects** — BTCUSD options strategy is private and must never appear on the site
- **Remove company-specific references** when repurposing research (e.g., Saama content pending review)
- **All content edits** should be reflected in both the HTML prototype and (eventually) the Astro source files
- **Maintain warm-gravitas tone** — professional, global, approachable. Not intimidating. Not generic.
- **Single HTML file** for now — `outputs/index.html` is the source of truth until Astro is set up

---

## File Structure (Current)
```
outputs/
├── index.html          ← Main landing page (single file, self-contained)
└── PROJECT_CONTEXT.md  ← This file
```

## File Structure (Target — Astro)
```
karanam-ai/
├── src/
│   ├── pages/
│   │   └── index.astro
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Expertise.astro
│   │   ├── Timeline.astro
│   │   ├── Recognition.astro
│   │   └── Contact.astro
│   └── styles/
│       └── global.css
├── public/
├── astro.config.mjs
├── package.json
├── HOWTO.md            ← Plain-English guide for Manohar to make updates
└── README.md
```
