# FitHub Support Page

This repository contains the support page for FitHub app.

## Setup Instructions

1. Create a new GitHub repository (e.g., `fithub-support` or `fithub-app.com`)
2. Push this folder to the repository
3. Go to repository Settings > Pages
4. Select the `main` branch and `/ (root)` folder
5. Your support page will be available at `https://[username].github.io/[repo-name]`
6. To use your custom domain `fithub-app.com`, add it in the Pages settings

## Custom Domain Setup

1. In GitHub Pages settings, add your custom domain: `fithub-app.com`
2. Add a CNAME file (GitHub will create this automatically)
3. Update your domain's DNS records:
   - Add an A record pointing to: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - OR add a CNAME record pointing to: `[username].github.io`

## Files

- `index.html` - The support page (renamed from support.html for GitHub Pages)
