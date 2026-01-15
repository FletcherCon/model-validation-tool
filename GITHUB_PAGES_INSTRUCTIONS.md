# How to Publish to GitHub Pages

## Files You Need
- `index.html` - The main documentation page
- `README.md` - Repository description
- `.nojekyll` - Empty file (create this in your repo)

---

## Option 1: Using GitHub Web Interface (Easiest)

### Step 1: Create a New Repository
1. Go to https://github.com/new
2. Enter a repository name (e.g., `model-validation-docs`)
3. Set to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### Step 2: Upload Files
1. Click **"uploading an existing file"** link
2. Drag and drop `index.html` and `README.md`
3. Click **Commit changes**

### Step 3: Create .nojekyll File
1. Click **Add file** → **Create new file**
2. Name it `.nojekyll` (just the filename, leave content empty)
3. Click **Commit new file**

### Step 4: Enable GitHub Pages
1. Go to **Settings** → **Pages** (in left sidebar)
2. Under "Source", select **Deploy from a branch**
3. Select **main** branch and **/ (root)** folder
4. Click **Save**

### Step 5: Access Your Site
After 1-2 minutes, your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

---

## Option 2: Using Git Command Line

```bash
# 1. Create a new directory and initialize git
mkdir model-validation-docs
cd model-validation-docs
git init

# 2. Copy your files into this directory
# - index.html
# - README.md

# 3. Create .nojekyll file
touch .nojekyll

# 4. Add and commit files
git add .
git commit -m "Initial commit - Model Validation Tool documentation"

# 5. Create repository on GitHub first, then:
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main

# 6. Enable GitHub Pages in repository Settings → Pages
```

---

## Sharing with Your Team

Once published, share this link with your BIM team:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

They can view it in any web browser without needing GitHub accounts.

---

## Updating the Documentation

To update the page later:
1. Edit `index.html` on GitHub (click the file → pencil icon)
2. Or upload a new version (Add file → Upload files)
3. Changes go live within 1-2 minutes

---

## Troubleshooting

**Page not loading?**
- Wait 2-5 minutes after enabling Pages
- Check Settings → Pages for any error messages
- Ensure the repository is Public

**Styles not showing?**
- Make sure `.nojekyll` file exists in the root
- Clear your browser cache (Ctrl+Shift+R)

**404 Error?**
- Ensure file is named exactly `index.html` (lowercase)
- Check that Pages is enabled on the correct branch
