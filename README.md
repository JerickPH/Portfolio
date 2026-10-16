# Jerick Paler – Portfolio

Static site: `index.html` + `assets/`. No build step.

## Add your photo
1. Put your photo in `assets/` (e.g. `assets/profile.jpg`, portrait, about 600×720 or larger).
2. In `index.html`, find `assets/profile-placeholder.svg` and change it to `assets/profile.jpg`.

Note: `assets/` is cached for a year. If you later replace the photo, use a new file name (e.g. `profile-2.jpg`).

## Deploy to Vercel

**Option A – GitHub (recommended, auto-deploys on every push)**
1. Create a new GitHub repo and upload these files (keep `index.html` at the root).
2. Go to vercel.com → Add New → Project → import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty. Click Deploy.

**Option B – Vercel CLI**
```
npm i -g vercel
cd jerick-portfolio
vercel        # preview
vercel --prod # production
```

## Edit content
All text lives in `index.html`. Sections are marked with comments: HERO, SERVICES, WORK, PROCESS, ABOUT, CONTACT.
To add a project, copy one `<details class="case">` block. Its `data-cat` (automation / voice / web) controls the filter buttons.
