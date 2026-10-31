# Shruti Pandey personal site: context for Claude

Public Jekyll site on GitHub Pages (live at https://shrutinmpandey.github.io/, repo `shrutinmpandey/shrutinmpandey.github.io`). Built by Aryan for Shruti. See `README.md` for run and edit instructions.

## Working rules

- Commit and push to `main` after every change, without asking. Pushing deploys the site.
- Never put Claude or co-author attribution in commit messages.
- Never put her phone number on the site or in any committed file. `resume/` and `*.docx` are in `.gitignore` for this reason; keep them there.
- Per Aryan's global rule, discuss the approach before any substantive change.
- Run locally with Ruby 3.3.0 (`.ruby-version`): `bundle exec jekyll serve`. The system Ruby is too old.

## Structure

- `_config.yml` holds the name, tagline, email, LinkedIn and resume links. Reference them as `site.<key>`; add new personal details here.
- `_data/*.yml` holds the content: experience, education, awards, projects, certifications, volunteering, logos.
- Pages: `index.md`, `experience.md`, `education.md`, `awards.md`, `projects.md`. The header is in `_includes/header.html`.
- A script in `_layouts/default.html` makes every link open in a new tab.
- Light/dark theme in `assets/css/style.css`, with a toggle and system default.
- `resume/resume.tex` is for Overleaf, written to fit one page (never compiled locally, no LaTeX installed). It has a `PHONE-NUMBER` placeholder. If it overflows, switch to `\documentclass[9pt]{extarticle}`.

## Content decisions

- LinkedIn is the source of truth for projects, certifications and volunteering (copied as shown, 10 projects). Language proficiency and similar filler are left out.
- VIT Vellore education has two separate bullets: "Completed 12 projects" and "Featured in the official video...".
- The Reliance "~4 Cr/ton/year" figure is left off the website because it is ambiguous. It is in the resume tex as "INR 4 Cr per ton per year".
- Resume edits made: removed graVITas'22, the language row and the plain "Achievers Award" (kept "Special Achievers Award"), and removed the % for MBA and B.Tech.
- Her email, `shrutinmpandey@gmail.com`, was inferred from the old Google Site's Gmail link and from her CV.
- Resume link: Google Drive file (`resume_url` in `_config.yml`). It must stay shared as "anyone with the link can view".

## Open items and next steps

- Later: rework the resume and site to appeal to HR roles. She is an MBA (HR) with HR consulting and talent strategy experience at EY, Lenovo and Hinduja, so lead with that and move the chemical engineering material lower.
- Logos: the home page banner strip shows company names as text. Real logos need downloading trademarked image files, which needs Aryan's explicit go-ahead.
- The CV has details the site lacks: the Cipla internship (May-Jun 2022), the "Senior Placement Coordinator" title (the site says "Placement Coordinator"), the HR Analytics (UC Irvine) and Diversity and Inclusion (ESSEC) certifications, interests, and the AI-powered evaluation framework in the Hinduja work.
- The home page intro is a draft written from LinkedIn facts, and Shruti has not approved the wording.
