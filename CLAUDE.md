# Cyber-RN Blog — Project Context for Claude Code

## Who I Am
KC Felder (she/her), also goes by KC. BSN, RN, clinical informaticist, MSCSIA student at WGU focusing on GRC. 21 years in high-acuity clinical environments (ER, PACU, Surgical Services). Transitioning into cybersecurity. Not a developer — explain technical things through a security and clinical lens.

## What This Site Is
Personal cybersecurity blog at cyber-rn.github.io (GitHub Pages, static HTML/CSS, no build system).
- Dark theme, monospace-adjacent aesthetic
- CSS variables in `css/style.css` — always check there before adding styles
- All pages share the same header/footer/nav structure
- Google Analytics: G-4M5VVRE098 — add to every new page in `<head>` before `</head>`

## Site Structure
- `index.html` — homepage: hero → My Story section → Recent Posts list
- `about.html` — about page
- `posts/` — individual post pages
- `css/style.css` — single stylesheet for everything

## My Story Section
Permanent section on the homepage between the hero and the post list. Never remove or move it. It is KC's origin story — the car accident, Crohn's diagnosis, and nurse Kim who shaped her career. No key takeaway. No edits without KC's direction.

## Adding a New Post
1. Create `posts/your-post-slug.html` using the existing post pages as a template
2. Add the GA tag to `<head>`
3. Add a post card to `index.html` at the top of `.post-list` (newest first)
4. Commit and push to main — GitHub Pages deploys automatically

## Google Analytics Tag
```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-4M5VVRE098"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-4M5VVRE098');
</script>
```

## Writing Style
KC writes her own posts. Do not ghost-write unless explicitly asked. When helping:
- Her voice is direct, clinical, and specific — no fluff
- She uses concrete detail over abstraction
- Healthcare analogies are natural to her, not forced
- No key takeaways on personal/narrative posts; yes on technical posts
- No bullet-point summaries of her own writing back to her

## Current AI on This Session
If working from the laptop: this CLAUDE.md is your primary context. The full memory system lives on the PC. Brief yourself from this file and the git log.
