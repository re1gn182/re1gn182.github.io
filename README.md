# re1gn182.github.io

Personal portfolio site for Logan King — Cybersecurity Analyst (SOC, incident response, threat hunting, threat intelligence).

## Structure

```
re1gn182-site/
├── index.html              # the whole site (single page, inline CSS/JS)
├── assets/
│   └── Logan_King_Resume.pdf   # downloadable resume linked from the site
└── README.md
```

## Deploying to GitHub Pages

Since this repo is named `re1gn182.github.io`, GitHub will publish it automatically as a **user site** once you push it — no extra Pages configuration needed, as long as `index.html` sits at the repo root (it does).

1. Create the repository on GitHub (if you haven't already):
   - Go to github.com → New repository
   - Name it exactly `re1gn182.github.io`
   - Leave it public, and don't initialize with a README (you already have one here)

2. From this folder, push it up:
   ```bash
   cd re1gn182-site
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/re1gn182/re1gn182.github.io.git
   git push -u origin main
   ```

3. Give it a minute or two, then visit **https://re1gn182.github.io** — it should be live.

   If it doesn't show up right away, check the repo's **Settings → Pages** tab and confirm the source is set to deploy from the `main` branch, root folder.

## Editing later

- All content lives directly in `index.html` — text, styling, and layout are all in that one file, so updates are just editing the relevant `<section>` and pushing again.
- To update your resume file, replace `assets/Logan_King_Resume.pdf` with a new export using the same filename (or update the link paths in `index.html` if you rename it).

## A privacy note

Your phone number was on the resume PDF you're linking to, but I left it out of the page text itself since this site will be public and indexed by search engines. If you'd rather keep the phone number off the downloadable PDF too, swap in a version of the resume without it, or add a Google Voice-style number instead.
