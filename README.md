# TKH Tek Website Setup Guide (100% Free Forever)

This folder contains the complete, modern, responsive website for **TKH Tek** and **ChronoLens**:
- `index.html`: Clean dark-mode landing page showcasing ChronoLens, key features, and App Store links.
- `privacy.html`: In-depth, Apple App Store-compliant Privacy Policy page.
- `app-icon.png`: High-resolution ChronoLens app icon.

---

## Deploy to Cloudflare Pages (Easiest - 60 Seconds)
1. Go to [pages.cloudflare.com](https://pages.cloudflare.com) and create a free account.
2. Click **Create Application** > **Pages** > **Upload Assets**.
3. Drag and drop the `tkhtek-website` folder directly into Cloudflare.
4. Go to **Custom Domains** and add `tkhtek.com`.
5. Cloudflare will automatically provision a free SSL certificate!

---

## Deploy to GitHub Pages
1. Create a free repository on GitHub called `tkhtek-website`.
2. Push or upload the contents of this folder to the repository:
   ```bash
   cd tkhtek-website
   git init
   git add .
   git commit -m "Initial launch of TKH Tek site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/tkhtek-website.git
   git push -u origin main
   ```
3. In GitHub repo **Settings > Pages**:
   - Source: Deploy from a branch (`main` / root).
   - Custom Domain: Enter `tkhtek.com`.

---

## Point Squarespace DNS to Your Free Site

In your **Squarespace Domain Dashboard** (`tkhtek.com` > DNS Settings):

### If Using GitHub Pages:
Add these 4 **A Records** (Host: `@`):
- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Add one **CNAME Record**:
- Host: `www`
- Value: `YOUR_GITHUB_USERNAME.github.io`

### If Using Cloudflare Pages:
Cloudflare will give you a single CNAME record to paste into your Squarespace DNS.
