# GitHub Pages Setup Guide

Follow these steps to deploy your portfolio website to GitHub Pages.

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Name your repository (e.g., `portfolio` or `safe-saeed-portfolio`)
5. Choose **Public** (required for free GitHub Pages)
6. **DO NOT** initialize with README, .gitignore, or license (we already have these)
7. Click **Create repository**

## Step 2: Initialize Git and Push Files

Open PowerShell or Command Prompt in your project folder (`C:\Users\safe\Desktop\port`) and run:

```powershell
# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository (replace YOUR_USERNAME and YOUR_REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Important:** Replace `YOUR_USERNAME` with your GitHub username and `YOUR_REPO_NAME` with your repository name.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** (top menu)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

## Step 4: Access Your Live Website

After a few minutes, your website will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

For example, if your username is `safesaeed` and repo is `portfolio`:
```
https://safesaeed.github.io/portfolio/
```

## Updating Your Website

Whenever you make changes:

```powershell
git add .
git commit -m "Update portfolio"
git push
```

Changes will be live within 1-2 minutes!

## Troubleshooting

- **404 Error**: Wait a few minutes after enabling Pages, it takes time to deploy
- **Styles not loading**: Make sure all file paths are correct (case-sensitive)
- **Authentication issues**: You may need to use a Personal Access Token instead of password

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/en/pages
- Git Documentation: https://git-scm.com/doc

