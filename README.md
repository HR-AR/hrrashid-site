# personal-site — hrrashid.com

Personal portfolio site for Hakeem Rashid. Built via Claude Design AI (Opus 4.7), exported as standalone HTML.

## Current state (2026-05-25)

- ✅ `index.html` — 1.75MB standalone React bundle from Claude Design (Operator variant locked)
- ✅ `CNAME` — `hrrashid.com` for GitHub Pages
- ⬜ `assets/` — empty, will hold final headshot + og-image + favicon
- ⬜ GitHub repo not yet created (Phase 7)
- ⬜ DNS not yet configured at registrar (Phase 7)

## Preview locally

```bash
cd /Users/hr2/1-Projects/work-life/personal-site
python3 -m http.server 8123
# Open http://localhost:8123/
```

## Architecture

Single-file bundle. All HTML + CSS + JS + content inline. Renders identically to what was generated in Claude Design.

Sections (in order, all rendered):
1. Sticky top nav (HR badge + name + 10 anchor links + Get in touch CTA)
2. Hero — locked copy: "As Director of Last Mile Delivery Technology at Walmart, I run logistics networks handling 100,000 deliveries a day. Behind the scenes, I'm a hands-on AI workflow builder coding Atlas harnesses, Hermes goals, and NotebookLM-driven research pipelines. I open-source my exact methodology on LinkedIn and The Flow Architect YouTube channel."
3. 3 stat callouts in JetBrains Mono: `100K` deliveries/day · `5,000` stores in 5 weeks · `2` AI harnesses
4. Dual CTAs: "See AI Builds" (cyan filled) + "Get in Touch" (cyan outline)
5. Terminal-style portrait window — placeholder `portrait.jpg` with name/role/base/status
6. About (3-column copy)
7. What I Do — 8 competencies grid
8. AI Builds — 6 LinkedIn build cards
9. The Flow Architect YouTube section
10. Featured Writing & Socials
11. Career Experience timeline (placeholder content for prior roles)
12. How I Work — 5 cited leadership principles
13. Case Studies (01 OS+Reg, 02 Nash 5K stores, 03 AI Architecture)
14. Speaking & Press
15. Contact footer

## Visual system (locked)

- **Palette**: Flow Architect — navy `#1a1a2e` bg, cyan `#00d4ff` accent, warm white `#f5f5f5` text, emerald `#00c48c` metrics
- **Typography**: Inter for body/headings, JetBrains Mono for stat callouts and terminal styling
- **Variant**: Operator (Inter 800 headlines, dense card grid, balanced cyan)

## What's still TODO

| # | Item | Phase |
|---|---|---|
| 1 | Swap `portrait.jpg` placeholder for real headshot | 4a (deferred) |
| 2 | Fill prior-role timeline content (currently placeholder) | 5 |
| 3 | Real GitHub URLs in AI Builds cards (currently `github.com/HR-AR/*`) | 5 |
| 4 | Anti-slop pass on body copy | 5 |
| 5 | Fresh-context review via `/review-draft --slop --strategic` | 5 |
| 6 | LinkedIn article dossier for Featured section approvals | 5 |
| 7 | Apply LINKEDIN_OPTIMIZATION_PACKAGE.md via Claude in Chrome | 6 |
| 8 | Create GitHub repo + push site + DNS setup at registrar | 7 |
| 9 | Schedule Hermes goal for 1-week analytics check | 8 |
| 10 | Session close-out + MEMORY.md update | 8 |

## DNS records to add at hrrashid.com registrar (Phase 7)

- `CNAME` record: `www` → `<github-username>.github.io`
- `A` records on apex (4 of them):
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`

GitHub Pages auto-provisions HTTPS cert 5 min – 24 h after DNS resolves.

## Source artifacts

- Claude Design project: https://claude.ai/design/p/d908ecd1-7efc-4413-be39-8da1176f4860
- Design prompt: `/tmp/claude-design-prompt-hrrashid.md` (240 lines)
- Build artifact log: `01-projects/engagement/content-pipeline/claude-design/hrrashid-portfolio-2026-05-25.md`
- Recruiter-POV research: `00-inbox/recruiter-pov-findings.md`
- Voice synthesis output: `00-inbox/personal-brand-voice-synthesis.md`
- NotebookLM notebooks:
  - `recruiter-pov-portfolio` — `b3936f5a-326d-4b4e-8b9d-7fda61155b2f` (17 sources)
  - `personal-brand-hakeem` — `42c24b19-188c-496f-80b6-c8bec99806f1` (10 sources)
