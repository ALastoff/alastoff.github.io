# Setup Instructions for alastoff.github.io

Your portfolio website is ready! Follow these steps to get it live on GitHub.

## Prerequisites

1. **Git for Windows**: Download and install from https://git-scm.com/download/win
2. **GitHub Account**: You already have one at https://github.com/alastoff

## Step-by-Step Setup

### 1. Initialize Git Repository Locally

Open PowerShell and run:

```powershell
cd "C:\Users\Administrator\Documents\GitHub-Portfolio"
git init
git add .
git commit -m "Initial commit: Portfolio website with projects showcase"
```

### 2. Create Repository on GitHub

1. Go to https://github.com/new
2. **Important**: Repository name MUST be exactly: `alastoff.github.io`
3. Set as **Public** (required for GitHub Pages)
4. DO NOT add README, .gitignore, or license (we already have these)
5. Click "Create repository"

### 3. Connect Local Repository to GitHub

In PowerShell, run these commands:

```powershell
# Add the remote repository
git remote add origin https://github.com/alastoff/alastoff.github.io.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

When prompted for credentials:
- **Username**: alastoff
- **Password**: Use your GitHub Personal Access Token (or GitHub CLI)

### 4. Enable GitHub Pages (Usually Automatic)

GitHub Pages will automatically activate for your repository. In about 1-2 minutes, your site will be live at:

**https://alastoff.github.io**

## What You Get

✅ Professional portfolio website
✅ Project showcase cards for:
   - Zerto Licensing Utilization Report
   - SQL Server TempDB Optimization
✅ Skills section
✅ Contact/social links
✅ Responsive design (works on all devices)
✅ Custom animations and gradients
✅ Print-friendly styling

## File Structure

```
alastoff.github.io/
├── index.html          # Main portfolio page
├── assets/
│   └── css/
│       └── styles.css  # Custom styling
├── README.md           # Documentation
└── .gitignore          # Git ignore rules
```

## Making Updates

To update your portfolio in the future:

```powershell
cd "C:\Users\Administrator\Documents\GitHub-Portfolio"

# Make your changes to files

# Stage and commit
git add .
git commit -m "Update: Your change description"

# Push to GitHub
git push origin main
```

Changes typically appear within 1-2 minutes.

## Customization

### Update Personal Info
Edit `index.html` and look for these sections:
- LinkedIn URL: line ~228
- Email: line ~229
- GitHub URL: appears multiple times

### Add More Projects
1. Find the "Projects Section" in index.html (around line ~130)
2. Copy one of the project card `<div>` blocks
3. Update the project details
4. Save and commit

### Modify Colors
Edit `assets/css/styles.css` and change the color variables:
```css
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --success-color: #10b981;
}
```

## Troubleshooting

### "Git not found"
Install Git for Windows: https://git-scm.com/download/win

### Repository creation failed
Make sure your repository name is EXACTLY: `alastoff.github.io`

### Site not showing up
1. Check repository settings → Pages section
2. Confirm branch is set to "main"
3. Wait 1-2 minutes and refresh browser
4. Try a hard refresh: Ctrl+Shift+Delete or Cmd+Shift+Delete

### Want custom domain?
In GitHub repository settings → Pages, add your custom domain (requires DNS setup)

## Next Steps

1. Install Git for Windows
2. Create repository on GitHub
3. Run the git commands above
4. Visit https://alastoff.github.io
5. Share your portfolio! 🚀

---

For more GitHub Pages info: https://pages.github.com/
