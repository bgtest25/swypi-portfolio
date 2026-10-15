# Portfolio Showcase

This folder contains public-safe materials for showcasing my work.

## Contents

- `SWYPI-CASE-STUDY.md` - Technical case study of the Swypi social platform

## How to Use

### Option 1: Create a Public GitHub Repo

```bash
# Create a new public repo on GitHub called "portfolio" or "projects"
# Then from this folder:
cd portfolio
git init
git add .
git commit -m "Add Swypi case study"
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git push -u origin main
```

### Option 2: Add to Existing Portfolio Repo

Copy these files to your existing portfolio/projects repository.

## Security Checklist

Before pushing to a public repo, verify:

- [ ] No `.env` files or secrets
- [ ] No API keys or tokens
- [ ] No database connection strings
- [ ] No proprietary business logic or code
- [ ] No user data or PII references
- [ ] No internal URLs or endpoints

This folder is designed to be copied out of the main project repo, NOT to make the main repo public.

## Adding More Projects

Create additional `PROJECT-NAME-CASE-STUDY.md` files following the same format.
