# 🚀 Deployment Guide

This guide will help you deploy your portfolio website to GitHub Pages.

## Prerequisites

- GitHub account
- Git installed on your computer
- Your portfolio files ready

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com)
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name it: `prayaschavda.github.io` (replace with your GitHub username)
5. Make sure it's **Public**
6. **Don't** initialize with README, .gitignore, or license (we already have these)
7. Click "Create repository"

## Step 2: Upload Your Files

### Option A: Using GitHub Web Interface (Easiest)

1. On your new repository page, click "uploading an existing file"
2. Drag and drop all your portfolio files
3. Write a commit message: "Initial portfolio upload"
4. Click "Commit changes"

### Option B: Using Git Command Line

1. Open terminal/command prompt in your portfolio folder
2. Run these commands:

```bash
git init
git add .
git commit -m "Initial portfolio upload"
git branch -M main
git remote add origin https://github.com/prayaschavda/prayaschavda.github.io.git
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

## Step 4: Access Your Website

Your website will be available at:
`https://prayaschavda.github.io`

⚠️ **Note**: It may take a few minutes for the site to become available.

## Step 5: Custom Domain (Optional)

If you have a custom domain:

1. In your repository, create a file named `CNAME`
2. Add your domain name (e.g., `prayaschavda.com`)
3. In your domain provider's settings, add a CNAME record pointing to `prayaschavda.github.io`

## Updating Your Website

To update your website:

1. Make changes to your files
2. Commit and push changes:

```bash
git add .
git commit -m "Update portfolio"
git push
```

The changes will be live within a few minutes.

## Troubleshooting

### Website not loading
- Check if GitHub Pages is enabled in repository settings
- Ensure your main file is named `index.html`
- Wait a few minutes as deployment takes time

### Images not showing
- Make sure image paths are relative (e.g., `./images/photo.jpg`)
- Check file names for correct capitalization

### Custom domain not working
- Verify CNAME file content
- Check DNS settings with your domain provider
- Allow up to 48 hours for DNS propagation

## Performance Tips

1. **Optimize Images**: Compress images before uploading
2. **Minify Code**: Consider minifying CSS and JavaScript for faster loading
3. **CDN**: Use CDN links for libraries (already done with Tailwind and GSAP)

## Security

- Never commit sensitive information (API keys, passwords)
- Use environment variables for sensitive data
- Keep dependencies updated

## SEO Optimization

Your portfolio already includes:
- Meta tags for social sharing
- Semantic HTML structure
- Fast loading times
- Mobile responsiveness

## Need Help?

If you encounter issues:
1. Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
2. Look for solutions in GitHub Community
3. Contact support if needed

---

**Good luck with your portfolio deployment! 🎉**
