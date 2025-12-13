# GitHub Repository Setup Instructions

Follow these steps to push this repository to GitHub.

---

## Step 1: Initialize Git Repository

In your terminal, navigate to the repository folder and initialize git:

```bash
cd /path/to/forteen-mind-labs-repo
git init
```

---

## Step 2: Add All Files

Add all files to git tracking:

```bash
git add .
```

---

## Step 3: Create Initial Commit

```bash
git commit -m "Initial commit: FORTEEN MIND LABS - Episode 1 complete"
```

---

## Step 4: Create GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the **"+"** icon in top right
3. Select **"New repository"**
4. Configure your repository:
   - **Repository name**: `forteen-mind-labs` (or your preferred name)
   - **Description**: "Forteen Mind Labs - A premium micro-learning series exploring human behavioral patterns"
   - **Visibility**: 
     - Choose **Private** if you want to keep it confidential
     - Choose **Public** if you want to share it
   - **DO NOT** initialize with README (we already have one)
5. Click **"Create repository"**

---

## Step 5: Connect Local to GitHub

GitHub will show you commands. Use the "push an existing repository" section:

```bash
git remote add origin https://github.com/YOUR-USERNAME/forteen-mind-labs.git
git branch -M main
git push -u origin main
```

**Replace `YOUR-USERNAME`** with your actual GitHub username.

---

## Step 6: Verify Upload

1. Refresh your GitHub repository page
2. You should see all files and folders
3. Check that README.md displays correctly
4. Verify folder structure matches local

---

## Alternative: Using GitHub Desktop

If you prefer a GUI:

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Open GitHub Desktop
3. File → Add Local Repository
4. Select the `forteen-mind-labs-repo` folder
5. Click "Publish repository"
6. Choose repository name and visibility
7. Click "Publish"

---

## Repository Structure You'll See on GitHub

```
forteen-mind-labs/
├── README.md
├── .gitignore
├── GITHUB_SETUP.md (this file)
├── docs/
│   ├── THE_UNDERTOW_Project_Bible.md
│   └── episode-1-guide.md
├── episodes/
│   ├── episode-1-full.html
│   └── episode-1-teaser.html
├── marketing/
│   └── forteen-mind-labs-poster.html
└── assets/
    ├── fonts/
    └── images/
```

---

## Future Updates

When you make changes and want to push them to GitHub:

```bash
# Check what's changed
git status

# Add specific files
git add filename.html

# Or add all changes
git add .

# Commit with a message
git commit -m "Description of what you changed"

# Push to GitHub
git push
```

---

## Branches (Optional)

For working on new features without affecting main:

```bash
# Create new branch
git checkout -b feature/episode-2

# Make changes, commit them
git add .
git commit -m "Work in progress: Episode 2"

# Push branch to GitHub
git push -u origin feature/episode-2

# When ready, merge on GitHub via Pull Request
```

---

## Recommended GitHub Settings

After creating the repository:

1. **Settings → General**:
   - Add topics: `education`, `psychology`, `micro-learning`, `behavioral-science`
   - Update description if needed

2. **Settings → Pages** (if you want to host):
   - Source: Deploy from branch
   - Branch: `main`, folder: `/` (root)
   - Your episodes will be live at: `https://YOUR-USERNAME.github.io/forteen-mind-labs/`

3. **Settings → Security** (if private repo):
   - Consider adding collaborators if working with a team

---

## Hosting on GitHub Pages (Optional)

If you want to make episodes publicly accessible via web:

1. Go to repository **Settings**
2. Click **Pages** in left sidebar
3. Under "Source", select **main** branch
4. Click **Save**
5. Wait a few minutes
6. Your site will be live at: `https://YOUR-USERNAME.github.io/forteen-mind-labs/`

Access episodes:
- Episode 1: `https://YOUR-USERNAME.github.io/forteen-mind-labs/episodes/episode-1-full.html`
- Teaser: `https://YOUR-USERNAME.github.io/forteen-mind-labs/episodes/episode-1-teaser.html`

---

## Troubleshooting

**Issue**: "Permission denied (publickey)"
- **Solution**: Set up SSH keys or use HTTPS URL with personal access token

**Issue**: Large files won't upload
- **Solution**: Check .gitignore, files over 100MB need Git LFS

**Issue**: Changes not showing on GitHub Pages
- **Solution**: Wait 5-10 minutes, then hard refresh browser (Cmd+Shift+R or Ctrl+Shift+R)

---

## Need Help?

- [GitHub Documentation](https://docs.github.com)
- [GitHub Desktop Guide](https://docs.github.com/en/desktop)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

---

**You're all set!** 🚀

Your FORTEEN MIND LABS project is now safely stored and version controlled on GitHub.
