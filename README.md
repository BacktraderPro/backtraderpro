# Backtrader Pro - GitHub Pages Website

This is the official website for Backtrader Pro, a professional trading strategy development and backtesting platform.

## 🚀 Setting Up GitHub Pages

Follow these steps to host this website on GitHub Pages:

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click the **+** icon in the top-right corner and select **New repository**
3. Name your repository (e.g., `backtrader-pro` or `backtrader-pro.github.io`)
4. Choose **Public** visibility
5. **Do NOT** initialize with README, .gitignore, or license (we already have files)
6. Click **Create repository**

### Step 2: Upload Your Website Files

You have two options:

#### Option A: Upload via GitHub Web Interface (Easiest)

1. In your new repository, click **uploading an existing file**
2. Drag and drop all the files from your local folder:
   - `index.html`
   - `getting-started.html`
   - `documentation.html`
   - `faq.html`
   - `style.css`
   - `README.md` (this file)
3. Scroll down and click **Commit changes**

#### Option B: Upload via Git Command Line

1. Open Terminal/Command Prompt
2. Navigate to the folder containing your website files
3. Run these commands (replace `YOUR_USERNAME` and `REPO_NAME`):

```bash
git init
git add .
git commit -m "Initial commit - Backtrader Pro website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, click **Settings** (top menu)
2. In the left sidebar, click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, select **main** and **/ (root)**
5. Click **Save**

### Step 4: Access Your Website

1. Wait 1-2 minutes for GitHub to build your site
2. Your website will be available at:
   - If repo name is `USERNAME.github.io`: `https://USERNAME.github.io`
   - Otherwise: `https://USERNAME.github.io/REPO_NAME`

For example:
- `https://yourusername.github.io/backtrader-pro`

## 📝 Updating Your Website

Whenever you make changes to your website:

### Via Web Interface:
1. Go to your repository on GitHub
2. Click on the file you want to edit
3. Click the pencil icon (Edit this file)
4. Make your changes
5. Scroll down and click **Commit changes**
6. Wait 1-2 minutes for changes to appear on your live site

### Via Git:
```bash
git add .
git commit -m "Description of your changes"
git push
```

## 📦 Adding Your App Files

To add your actual installer files:

### Option 1: GitHub Releases (Recommended for Large Files)

1. Go to your repository
2. Click **Releases** on the right sidebar
3. Click **Create a new release**
4. Tag version (e.g., `v1.0.0`)
5. Upload your installer files (BacktraderPro-Setup.exe, etc.)
6. Click **Publish release**
7. Update the download links in `index.html` to point to your release files

The download URL format will be:
```
https://github.com/USERNAME/REPO_NAME/releases/download/v1.0.0/BacktraderPro-Setup.exe
```

### Option 2: Direct Repository Files (For Small Files Only)

1. Upload files directly to the repository (< 25 MB per file)
2. Update download links in `index.html`:

```html
<a href="BacktraderPro-Setup.exe" download>Download for Windows</a>
```

## 🎨 Customization

### Update Download Links

Edit `index.html` and find the download section (search for `download-button`). Update the `href` attributes with your actual file URLs.

### Change Colors

Edit `style.css` and modify the CSS variables at the top:

```css
:root {
    --primary-color: #2563eb;  /* Main brand color */
    --primary-dark: #1e40af;   /* Darker shade */
    /* etc. */
}
```

### Add Your Logo

1. Upload your logo image to the repository
2. Edit `index.html` and replace the text brand with an image:

```html
<div class="nav-brand">
    <img src="logo.png" alt="Backtrader Pro" height="40">
</div>
```

### Update Content

Simply edit the HTML files to change text, add features, or update information.

## 📄 Files Included

- `index.html` - Homepage with features and download section
- `getting-started.html` - Installation and setup guide
- `documentation.html` - Complete documentation and user guide
- `faq.html` - Frequently asked questions
- `style.css` - Professional styling and responsive design
- `README.md` - Setup instructions (this file)

## 🔗 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Markdown Guide](https://guides.github.com/features/mastering-markdown/)

## 🆘 Troubleshooting

### Website not showing up?
- Wait 2-3 minutes after enabling GitHub Pages
- Check that GitHub Pages is enabled in Settings → Pages
- Verify your repository is Public
- Check that `index.html` is in the root directory

### Changes not appearing?
- Wait 1-2 minutes for GitHub to rebuild the site
- Try hard refresh (Ctrl+F5 or Cmd+Shift+R)
- Clear your browser cache

### 404 Error?
- Ensure file names match exactly (case-sensitive)
- Check that all files are in the root directory
- Verify internal links use correct file names

## 📞 Support

For issues with:
- **GitHub Pages**: Check [GitHub Docs](https://docs.github.com/en/pages)
- **Git/GitHub**: Visit [GitHub Help](https://help.github.com)
- **Website customization**: Edit the HTML/CSS files as needed

---

**Good luck with your Backtrader Pro website!** 🎉
