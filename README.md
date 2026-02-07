# Portfolio Content Update Checklist

Use this checklist when adding new certifications, projects, or achievements.

## 1) Pull latest changes

```bash
git checkout main
git pull origin main
```

## 2) Update content in `index.html`

- Profile summary:
  - Section: `#resume` -> `Summary`
  - Keep keywords ATS-friendly: `Data Migration`, `Data Quality`, `Data Governance`, `MDM`, `Informatica IDMC`, `Python`.
- Certifications:
  - Section: `#resume` -> `Selected Certifications`
  - Add certification name, issuer, and year/recency.
- Experience highlights:
  - Section: `#resume` -> `Professional Experience`
  - Keep bullets outcome-first (metric + impact).
- Project history:
  - Section: `#project-timeline`
  - Add project, role, location, and exact date range.
- Portfolio cards:
  - Section: `#portfolio`
  - Add title + image + filter category (`Migration`, `Governance`, `Architecture`).
- Skills:
  - Section: `#skills`
  - Update skill labels and percentages.
- Contact:
  - Section: `#contact`
  - Keep authoritative contact details here as single source of truth.

## 3) Keep design consistent (`assets/css/style.css`)

- Reuse existing classes first (avoid one-off styles).
- Use theme variables:
  - `--theme-purple`
  - `--theme-purple-deep`
  - `--theme-orange`
- Keep cards balanced with consistent spacing and border radius.

## 4) ATS writing rules

- Prefer clear job-title keywords in headings.
- Start bullets with action verbs: `Led`, `Architected`, `Implemented`, `Delivered`.
- Include measurable outcomes where possible.
- Avoid repeating phone/email in many sections.

## 5) Preview and validate

- Open site locally and check:
  - Desktop and mobile layout.
  - Sidebar visibility and no clipping.
  - Timeline alignment.
  - Link correctness (especially LinkedIn and portfolio links).

## 6) Commit and publish

```bash
git add index.html assets/css/style.css README.md
git commit -m "Update profile content and timeline"
git push origin main
```

## 7) Confirm deployment

- Wait ~1-3 minutes for GitHub Pages.
- Hard refresh browser: `Cmd+Shift+R`.
