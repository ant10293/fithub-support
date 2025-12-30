# Quick Deployment Guide

## Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Create a new repository (name it `fithub-support` or `fithub-app.com`)
3. **DO NOT** initialize with README, .gitignore, or license
4. Click "Create repository"

## Step 2: Initialize Git and Push

Run these commands in the `github-pages` folder:

```bash
cd /Users/anthonycantu/Desktop/iOS/FitHub/github-pages
git init
git add .
git commit -m "Initial commit: Support page"
git branch -M main
git remote add origin https://github.com/[YOUR_USERNAME]/[REPO_NAME].git
git push -u origin main
```

Replace `[YOUR_USERNAME]` and `[REPO_NAME]` with your actual GitHub username and repository name.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

Your page will be live at: `https://[YOUR_USERNAME].github.io/[REPO_NAME]`

## Step 4: Add Custom Domain (Optional)

To use `fithub-app.com`:

1. In Pages settings, add your custom domain: `fithub-app.com`
2. GitHub will create a `CNAME` file automatically
3. Update your domain's DNS:
   - **Option A (A Records)**: Add 4 A records:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **Option B (CNAME)**: Add CNAME record:
     - Name: `@` or `www`
     - Value: `[YOUR_USERNAME].github.io`
4. Wait for DNS propagation (can take up to 24 hours)
5. Check "Enforce HTTPS" in Pages settings once DNS is configured

## That's it!

Your support page should be live within a few minutes.

