# Return California — Site Preview & Publishing Guide

> **IMPORTANT REMINDER:**
> Pushing updates to **`main`** only updates your **GitHub preview**.
> **Your live Cloudflare website will NOT update automatically!**

---

## Your Two Links

- **Preview Site (GitHub Pages — updates when you push to `main`):**
  https://bkrawitz101.github.io/ReturnCalifornia/
- **Publish Live Page (GitHub — merges `main` into `production` for Cloudflare):**
  https://github.com/bkrawitz101/ReturnCalifornia/compare/production...main

---

## Step-by-Step Workflow

### 1. Make changes & preview on GitHub (safe — does NOT change live site)
1. Edit your site files (such as `index.html`).
2. Commit and push your changes to **`main`**:
   ```bash
   git add .
   git commit -m "Describe your update"
   git push origin main
   ```
3. Wait ~1 minute, then check your preview site:
   https://bkrawitz101.github.io/ReturnCalifornia/

### 2. Publish to your live Cloudflare website (manual step)
Only do this when your GitHub preview looks good and you're ready for everyone to see it:

1. Open the compare link:
   https://github.com/bkrawitz101/ReturnCalifornia/compare/production...main
2. Click **"Create pull request"** (give it any short title, like `Publish site updates`).
3. Click **"Merge pull request"** → **"Confirm merge"**.
4. Cloudflare will automatically deploy the **`production`** branch to your live website within ~1 minute.

---

## Quick Check: Do I have unpublished changes?
Whenever you open https://github.com/bkrawitz101/ReturnCalifornia and see a banner on `main` that says:
> *"This branch is X commits ahead of `production`."*

…that means you have updates on your GitHub preview that have **not** been pushed live to Cloudflare yet.
