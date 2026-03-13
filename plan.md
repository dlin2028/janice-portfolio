# Portfolio Website Plan — Janice Jiang

## 1. Overview & Goals

Build a polished, professional personal portfolio website for Janice Jiang — a CPA-licensed accountant, UIUC Gies graduate with dual 4.0 GPAs, and XBRL Postgraduate Technical Assistant at the FASB. The site should read like a high-end professional showcase, not a developer portfolio.

**Primary audience:** Recruiters at Big 4/public accounting firms, standard-setters (PCAOB, SEC, IASB), academic institutions for PhD or research roles, professional network contacts.

**Core message:** Exceptional academic achiever with rare technical depth (XBRL, Python, data analytics) in accounting standards — bridging traditional financial reporting with modern data infrastructure.

---

## 2. All Extracted Profile Data

### Identity
| Field | Value |
|---|---|
| Name | Janice Jiang |
| Title | Postgraduate Technical Assistant at the FASB |
| Location | 101 Washington St, Norwalk, CT 06854 |
| Email (FASB) | jjiang@fasb.org |
| Email (personal) | janicejiang683@gmail.com |
| Phone | (309) 839-3590 |
| LinkedIn | https://www.linkedin.com/in/janice-jiang-508bba21b/ |

### Bio (verbatim from LinkedIn About section)
> I studied accountancy at the University of Illinois at Urbana-Champaign, where I obtained both my Bachelor's and Master's degrees, with concentrations in financial reporting & assurance, and data analytics. I am currently the July 2025 to June 2026 XBRL Postgraduate Technical Assistant at the Financial Accounting Standards Board (FASB). I support the XBRL team in developing and maintaining the U.S. GAAP Taxonomy. Additionally, I am on the intangibles research project, and the Public Markets Advisory Committee (PMAC). To contact me, please email jjiang@fasb.org

### Experience

**1. Financial Accounting Standards Board (FASB)**
- Role: Postgraduate Technical Assistant
- Period: July 2025 – Present (Norwalk, Connecticut)
- Responsibilities:
  - Conduct technical research on revenue recognition issues and intangibles (particularly R&D costs); synthesize research findings and stakeholder feedback from comment letters and outreach calls into memoranda for Board deliberations
  - Perform data analytics on SEC filings to identify disclosure and tagging patterns; develop Python scripts to automate processing and validation of the U.S. GAAP Taxonomy using XBRL
  - Support the Public Markets Advisory Committee (PMAC) by preparing meeting materials, managing logistics, and drafting meeting minutes for semiannual meetings
  - Research and answer technical inquiries from practitioners related to the Accounting Standards Codification
  - Programmatically clean stakeholder outreach data to build visualizations for quarterly Chair reports
  - Present at public Board and advisory group meetings on technical accounting and digital reporting matters

**2. Caterpillar Inc.**
- Total tenure: 1 yr 4 mos, Peoria, Illinois

  **Internal Auditing & Advisory Services Intern** — May 2024 – Aug 2024 (4 mos)
  - Performed risk-based audit fieldwork in China: walkthroughs, inquiries, negotiations, sample testing, drafting workpapers & observations — with full Mandarin language support
  - Executed pre-fieldwork data analytics on auditee facility data to identify trends, outliers, and risk areas in ESG and supplier quality; built interactive Power BI dashboards to visualize findings
  - Used Python to analyze size distribution of 58,000+ files/folders in the Data Analytics team's shared drive; developed a Python tool to compare supplier data across multiple databases
  - Compiled and categorized total expenses for the internal audit team's annual training week over 2 years for benchmarking and future budgeting
  - Collaborated with risk consultants from Ernst & Young (25% of the internal audit team)

  **Competitive Intelligence Consulting Intern** — May 2023 – May 2024 (1 yr 1 mo)
  - Researched competitor websites, press releases, 10-K filings, and market research reports to gather insights on hundreds of competitors for strategic decision-making by senior management
  - Crafted professional PowerPoint slides on competitor activities: manufacturing footprints, dealer footprints, product portfolios, aftermarket practices, and market share
  - Specialized in Chinese competitors using Chinese-language sources; assisted in writing quarterly reports summarizing financials and strategic initiatives
  - Produced trend charts and footprint maps to visualize market trends and competitive landscape

**3. University of Illinois Urbana-Champaign**
- Role: Teaching Assistant
- Location: Champaign, Illinois
- Responsibilities:
  - Assisted professor in grading midterm exam, final project, and final exam
  - Hosted office hours around exam weeks
  - Course focused on fundamental Python and Excel skills

**4. Chinese Language and International Development Society (CLAID)**
- Total tenure: 2 yrs 9 mos, Champaign, Illinois

  **Vice President** — Apr 2023 – May 2024 (1 yr 2 mos)
  - Collaborated closely with the President to organize and lead board-wide meetings; oversaw board recruitment and club-wide events
  - Resolved internal conflicts, upheld professional behavior standards, and enforced CLAID's Constitution and Code of Conduct

  **Tutoring Branch Chair** — Aug 2022 – Apr 2023 (9 mos)
  - Oversaw all Tutoring Branch activities: managed branch members, recruited and coordinated tutors and learners, planned semesterly tutor workshops, led weekly Chinese conversation tables, and conducted one-on-one peer tutoring

  **Treasurer** — May 2022 – Apr 2023 (1 yr)
  - Controlled club financials

  **Tutoring Branch Board Member** — Sep 2021 – Aug 2022 (1 yr)
  - Supported tutoring program operations; communicated with Chinese international students about the tutoring program and tracked learner progress

### Education

**1. Master of Accounting Science — Gies College of Business, UIUC**
- Period: August 2024 – May 2025
- GPA: 4.0 / 4.0
- Concentrations: Financial Reporting & Assurance; Data Analytics

**2. Bachelor of Science, Accountancy — Gies College of Business, UIUC**
- Period: August 2021 – May 2024
- GPA: 4.0 / 4.0
- Honors: James Scholar, Bronze Tablet (Top 3% of graduating class)

### Skills & Certifications
**Technical Tools:**
- Python — pandas, numpy, matplotlib, statsmodels, scikit-learn, psycopg2, NLTK (LinkedIn Skill Assessment certified)
- Power BI
- Tableau
- SQL / pgAdmin
- GitHub / Visual Studio Code / JupyterLab
- CalcBench
- XBRL (eXtensible Business Reporting Language)
- Microsoft Excel, PowerPoint, Word

**Domain Expertise:**
- Financial Reporting & Assurance
- U.S. GAAP / Accounting Standards
- Data Analytics
- Audit & Internal Controls
- Accounting Standards Codification (ASC) research

**Credentials:**
- CPA (Certified Public Accountant) — all sections passed (2025)

### Languages
- Mandarin — Native
- English — Native
- Fuzhounese — Fluent

### Notable Achievements (from LinkedIn post, 97 reactions)
- Graduated with perfect transcripts (dual 4.0 GPA)
- Worked with notable figures in the accounting profession
- Passed all CPA exam sections (2025)
- Bronze Tablet — UIUC's highest academic honor (Top 3% university-wide)

---

## 3. Site Architecture

### Pages / Sections (single-page with anchor navigation recommended)

```
/ (home)
  ├── #hero         — Name, title, headshot, CTA buttons
  ├── #about        — Bio + "what I do" summary cards
  ├── #experience   — Timeline of roles
  ├── #education    — Degree cards with honors callouts
  ├── #skills       — Skills grid with icons
  ├── #achievements — Honors & highlights strip
  └── #contact      — Email, LinkedIn, contact form (optional)
```

A single-page layout (with smooth scroll) is best for this profile — it keeps the focus on content and works well as a digital resume sent to recruiters.

---

## 4. Section-by-Section Content Plan

### 4.1 Hero Section
```
[Large headshot photo]
Janice Jiang
XBRL Postgraduate Technical Assistant at the FASB | CPA | Gies UIUC ×2 — 4.0 GPA

[Button: View My Work]   [Button: Contact Me]
```
- Background: subtle professional texture or gradient (navy → deep teal)
- Font: large serif for name, clean sans-serif for subtitle
- Profile photo: circular crop, prominent sizing

### 4.2 About Section
**Headline:** "Bridging accounting standards and data."

Two-column layout:
- Left: Short punchy paragraphs adapted from LinkedIn bio
- Right: Three "highlight cards":
  - 🏛 FASB — U.S. GAAP Taxonomy
  - 🎓 UIUC Gies — Dual 4.0 GPA
  - 📊 CPA Licensed — All Sections Passed

**Body copy (adapted):**
> I'm an accountant with a deep interest in how financial data is structured, standardized, and communicated. At the Financial Accounting Standards Board, I work with the XBRL team to develop and maintain the U.S. GAAP Taxonomy — the backbone of structured financial reporting in the United States.
>
> My academic foundation at Gies College of Business shaped my dual focus: rigorous financial reporting & assurance, and data analytics. I believe the future of accounting lies at this intersection.

### 4.3 Experience Section
Timeline layout (vertical, left-aligned with company logo badges on right):

**Card 1 — FASB**
- Logo: FASB (image: `1631330709142`)
- Title: Postgraduate Technical Assistant
- Period: Jul 2025 – Present · Norwalk, CT
- Bullet points (pick 3–4 strongest for portfolio cards):
  - Develop Python scripts to automate processing and validation of the U.S. GAAP Taxonomy using XBRL
  - Conduct technical research on revenue recognition and R&D cost intangibles; synthesize findings into Board memoranda
  - Support the Public Markets Advisory Committee (PMAC): meeting materials, logistics, and minutes
  - Present at public Board and advisory group meetings on technical accounting and digital reporting

**Card 2 — Caterpillar Inc.**
- Logo: Caterpillar (image: `caterpillar_inc_logo`)
- Title: Internal Auditing & Advisory Services Intern / Competitive Intelligence Consulting Intern
- Period: May 2023 – Aug 2024 (1 yr 4 mos total) · Peoria, IL
- Bullet points:
  - Performed risk-based audit fieldwork in China — walkthroughs, sample testing, workpapers — with Mandarin language support
  - Researched competitors using 10-K filings, press releases, and market reports to inform senior management's strategic decisions

**Card 3 — UIUC Teaching Assistant**
- Logo: Gies/UIUC logo (image: `giesbusiness_logo`)
- Title: Teaching Assistant
- Location: Champaign, IL
- Bullet points:
  - Graded midterm exams, final projects, and final exams for undergraduate course
  - Hosted exam-week office hours to support student comprehension
  - Course content: foundational Python programming and Excel for accounting professionals

**Card 4 — Chinese Language and International Development Society (CLAID)**
- Logo: CLAID logo (image: `claiduiuc_logo`)
- Title: Vice President → Tutoring Branch Chair → Treasurer
- Period: Sep 2021 – May 2024 (2 yrs 9 mos) · Champaign, IL
- Bullet points:
  - Led board-wide meetings and oversaw club recruitment as Vice President; enforced CLAID's Constitution and Code of Conduct
  - Directed all Tutoring Branch operations: tutor/learner matching, workshops, weekly Chinese conversation tables, one-on-one peer tutoring
  - Managed club finances as Treasurer

### 4.4 Education Section
Two cards, side by side (or stacked on mobile):

**Card 1**
- Institution: Gies College of Business, University of Illinois Urbana-Champaign
- Degree: Master of Accounting Science (MAS)
- Period: Aug 2024 – May 2025
- GPA: 4.0 / 4.0
- Concentrations: Financial Reporting & Assurance · Data Analytics
- Logo: Gies/UIUC

**Card 2**
- Institution: Gies College of Business, University of Illinois Urbana-Champaign
- Degree: Bachelor of Science, Accountancy
- Period: Aug 2021 – May 2024
- GPA: 4.0 / 4.0
- Honors: 🏅 James Scholar · 🏆 Bronze Tablet (Top 3%)
- Logo: Gies/UIUC

### 4.5 Skills Section
Grid layout (3–4 columns), each cell has an icon + skill name + optional badge:

**Technical Tools:**
| Skill | Badge / Note |
|---|---|
| Python | LinkedIn Assessment Certified ⭐ |
| Power BI | |
| Tableau | |
| SQL | |
| XBRL | eXtensible Business Reporting Language |
| Microsoft Excel | |
| GitHub | |
| CalcBench | |

**Domain Expertise:**
| Skill | Badge / Note |
|---|---|
| Financial Reporting & Assurance | |
| U.S. GAAP | |
| Data Analytics | |
| Audit & Internal Controls | |

**Credentials & Languages:**
| Skill | Badge / Note |
|---|---|
| CPA | All sections passed — 2025 |
| Mandarin | Native |
| Fuzhounese | Fluent |

### 4.6 Achievements / Honors Strip
Horizontal band with 4 highlight tiles:

| Honor | Detail |
|---|---|
| CPA Licensed | All exam sections passed — 2025 |
| Bronze Tablet | Top 3% — UIUC University-wide |
| Dual 4.0 GPA | BS & MAS, Gies College of Business |
| U.S. GAAP Taxonomy | Contributor at FASB |

### 4.7 Contact Section
```
Let's connect.
jjiang@fasb.org
[LinkedIn Profile →]
[Send an Email →]
```
- Clean, minimal. No form required unless desired.
- Location: Norwalk, Connecticut
- Personal email (for non-FASB inquiries): janicejiang683@gmail.com
- Phone: (309) 839-3590 — display discretionary (omit from public site; include on downloadable resume)

### 4.8 Resume Download (Optional)
Consider adding a "Download Resume" button in Hero or Nav linking to a PDF of `janice_jiang_resume.txt`.
This is a common recruiter expectation and easy to add as a static file in `public/resume.pdf`.

---

## 5. Design System

### Color Palette
```
Primary    #1A2B4A   Dark navy (professionalism, trust)
Accent     #C9A84C   Gold (UIUC brand, achievement)
Light BG   #F8F9FB   Off-white (clean, airy)
Text       #1C1C1E   Near-black
Muted      #6B7280   Gray (secondary text, dates)
Highlight  #E8F0FE   Soft blue (hover states, badge bg)
```

### Typography
```
Headings:  "Playfair Display" (serif) — elegant, academic
Body:      "Inter" (sans-serif) — modern, readable
Mono/Tech: "JetBrains Mono" — for XBRL/Python snippets (optional)
```
Both fonts available free via Google Fonts.

Scale: 16px base, 1.6 line height. Generous whitespace throughout.

### Visual Aesthetic
- Think: consulting firm meets academic CV (McKinsey / Deloitte report aesthetic)
- NOT: developer portfolio (no terminal windows, dark themes, code animations)
- Clean editorial layout, used of horizontal rules and subtle section dividers
- Tasteful micro-animations: fade-in-up on scroll (Intersection Observer), no flashy effects
- Print-friendly layout (many recruiters print or PDF portfolios)

---

## 6. Recommended Tech Stack

### Option A — Recommended: SvelteKit + Bun + Tailwind CSS
```
Framework:   SvelteKit 2
Runtime/PM:  Bun
Styling:     Tailwind CSS v4
Deployment:  Cloudflare Pages / Netlify / Vercel
Fonts:       Self-hosted or Google Fonts via CSS
Images:      Optimized static assets in /static/images
```
**Pros:** Fast, SEO-friendly (SSG), minimal framework overhead, excellent DX with Bun tooling.

### Option B — Simpler: Plain HTML/CSS/JS
```
Styling:     Custom CSS (no framework)
Build:       None required
Deployment:  GitHub Pages or Netlify (free)
```
**Pros:** Zero dependencies, works anywhere, beginner-friendly.

### Option C — No-code: Framer or Webflow
**Pros:** Visual editor, excellent design quality, professional templates.
**Cons:** Monthly cost, less control, vendor lock-in.

**Recommendation: Option A (SvelteKit + Bun)** for the best balance of quality, performance, and long-term maintainability. Option B if minimal tooling is preferred.

---

## 7. File Structure (SvelteKit + Bun)

```
janice-portfolio/
├── static/
│   ├── images/
│   │   ├── profile.jpg          ← Janice's headshot (from LinkedIn file: 1754413121980)
│   │   ├── cover.jpg            ← Banner photo (from LinkedIn file: 1754413013917)
│   │   ├── fasb-logo.png        ← FASB logo (from LinkedIn file: 1631330709142)
│   │   ├── gies-logo.png        ← Gies UIUC logo (from LinkedIn file: giesbusiness_logo)
│   │   └── og-image.jpg         ← Social share preview (crop from cover or headshot)
│   └── favicon.ico
├── src/
│   ├── routes/
│   │   ├── +layout.svelte       ← Root layout (metadata shell + nav)
│   │   └── +page.svelte         ← Main page (assembles all sections)
│   ├── lib/
│   │   └── components/
│   │       ├── Nav.svelte
│   │       ├── Hero.svelte
│   │       ├── About.svelte
│   │       ├── Experience.svelte
│   │       ├── Education.svelte
│   │       ├── Skills.svelte
│   │       ├── Achievements.svelte
│   │       └── Contact.svelte
│   └── app.css                  ← Global styles + Tailwind directives
├── package.json
├── bun.lockb
├── tailwind.config.ts
├── svelte.config.js
├── vite.config.ts
└── tsconfig.json
```

---

## 8. Image Strategy

### Current Status
✅ **All images are present.** The `Janice Jiang _ LinkedIn_files/` directory exists in the workspace with all images saved as valid JPEG files.

### How to Copy Images to the Project
When setting up the SvelteKit project, copy files from `Janice Jiang _ LinkedIn_files/` to `static/images/` with proper extensions:

```bash
cp "Janice Jiang _ LinkedIn_files/1754413121980" static/images/profile.jpg
cp "Janice Jiang _ LinkedIn_files/1754413013917" static/images/cover.jpg
cp "Janice Jiang _ LinkedIn_files/1631330709142" static/images/fasb-logo.jpg
cp "Janice Jiang _ LinkedIn_files/giesbusiness_logo" static/images/gies-logo.jpg
cp "Janice Jiang _ LinkedIn_files/caterpillar_inc_logo" static/images/caterpillar-logo.jpg
cp "Janice Jiang _ LinkedIn_files/claiduiuc_logo" static/images/claid-logo.jpg
cp "Janice Jiang _ LinkedIn_files/university_of_illinois_at_urbana_champaign_logo" static/images/uiuc-logo.jpg
cp "Janice Jiang _ LinkedIn_files/1765420956947" static/images/recap-2025.jpg
```

Note: LinkedIn_files assets have no file extension but are valid JPEG files — renaming with `.jpg` is correct.

### Image Filenames → Usage Mapping
| LinkedIn filename | Intended use | Target path |
|---|---|---|
| `1754413121980` | Profile headshot | `public/images/profile.jpg` |
| `1754413013917` | Cover/banner photo | `public/images/cover.jpg` |
| `1631330709142` | FASB company logo | `public/images/fasb-logo.png` |
| `giesbusiness_logo` | Gies UIUC logo | `public/images/gies-logo.png` |
| `1765420956947` | 2025 recap post image | `public/images/recap-2025.jpg` |

### Fallback (if images unavailable)
- Profile photo: Professional placeholder with initials "JJ" in navy circle
- Logos: Fetch from official FASB / UIUC websites (check usage rights)
- FASB official logo: https://www.fasb.org (find in their press kit)
- Gies College logo: https://giesbusiness.illinois.edu

---

## 9. SEO & Metadata

```html
<title>Janice Jiang — XBRL Specialist & CPA | FASB</title>
<meta name="description" content="Janice Jiang is a CPA and XBRL Postgraduate Technical Assistant at the FASB, specializing in U.S. GAAP Taxonomy development, financial reporting, and data analytics. Gies College of Business, UIUC — dual 4.0 GPA." />

<!-- Open Graph (LinkedIn/social sharing) -->
<meta property="og:title" content="Janice Jiang — Portfolio" />
<meta property="og:description" content="CPA | FASB XBRL Postgraduate Technical Assistant | UIUC Gies 4.0" />
<meta property="og:image" content="/images/og-image.jpg" />
<meta property="og:type" content="website" />
```

---

## 10. Domain & Deployment

### Domain Options
- `janicejiang.com` — ideal, check availability
- `janicejiang.me` — professional alternative
- `jjiangcpa.com` — emphasizes CPA credential
- GitHub Pages subdomain: `[username].github.io/portfolio` (free, no custom domain needed)

### Deployment Steps (SvelteKit + Bun)
```bash
bunx create-svelte@latest janice-portfolio
cd janice-portfolio
bun install
# add components and content
git init && git add . && git commit -m "init"
# connect to GitHub, then deploy on Cloudflare Pages / Netlify / Vercel
```
Live in minutes with automatic HTTPS and CDN.

---

## 11. Implementation Phases

### Phase 1 — Foundation (Day 1)
- [ ] Initialize SvelteKit project with Bun + Tailwind
- [ ] Set up font imports (Playfair Display + Inter)
- [ ] Define color tokens in `tailwind.config.ts`
- [ ] Build `Nav`, `Hero`, and `Contact` Svelte components
- [ ] Deploy skeleton to Cloudflare Pages / Netlify / Vercel

### Phase 2 — Content Sections (Day 2–3)
- [ ] Obtain/optimize all images (see Image Strategy above)
- [ ] Build `About`, `Experience`, `Education`, `Skills` components
- [ ] Add scroll-based fade-in animations
- [ ] Implement `Achievements` strip

### Phase 3 — Polish (Day 4)
- [ ] Mobile responsiveness audit (especially timeline and grid layouts)
- [ ] SEO metadata and og:image
- [ ] Favicon and site manifest
- [ ] Accessibility audit (alt text, contrast ratios, keyboard nav)
- [ ] Performance audit (Lighthouse score ≥ 95)
- [ ] Connect custom domain (if purchased)

---

## 12. Inspiration & References

| Reference | What to borrow |
|---|---|
| [brittanychiang.com](https://brittanychiang.com) | Smooth scroll, sticky nav, section transitions |
| Deloitte / KPMG thought leadership pages | Clean editorial content layout |
| Harvard Law faculty pages | Academic profile formatting for education/honors |
| Linear.app marketing site | Micro-animations, subtle gradients |

**Key aesthetic rule:** Every design decision should feel at home in a Big 4 firm's annual report. Understated, precise, confident — not trendy or garish.
