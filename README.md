# Portfolio Website

A clean, minimal portfolio website built with HTML, CSS, and vanilla JavaScript.

## Features

- Responsive design (works on mobile, tablet, desktop)
- Smooth scrolling navigation
- Modal popups for project details
- Clean, professional styling
- No frameworks needed - just pure HTML/CSS/JS

## Files

- `index.html` - Main HTML structure
- `styles.css` - All styling and layout
- `script.js` - Interactive functionality (modals, smooth scrolling)

## Customization Guide

### 1. Update Your Information

**In `index.html`:**

Line 7: Update page title
```html
<title>Your Name - Communications & Marketing</title>
```

Lines 18-23: Update hero section with your name and tagline
```html
<h1>Your Name</h1>
<p class="tagline">Your Title/Role</p>
<p class="subtitle">Your value proposition</p>
```

Lines 135-155: Update About section with your background

Lines 166-168: Update contact links
```html
<a href="mailto:your.email@example.com" class="contact-button">Email Me</a>
<a href="https://linkedin.com/in/yourprofile" target="_blank" class="contact-button secondary">LinkedIn</a>
```

### 2. Add Your Projects

Each project has two parts:
1. **Project card** (in the grid) - shows preview
2. **Modal** (popup) - shows full details

**To edit a project:**
Find the project card section (around lines 35-75) and update:
- Project title
- Description
- Tags
- Modal ID

Then find the matching modal (around lines 182-220) and update:
- The Brief
- My Role
- The Approach
- Results

**To add more projects:**
Copy an entire project-card div and modal div, give them new IDs (modal5, modal6, etc.)

### 3. Add Images

Replace placeholder images:

Option A: Use actual images
```html
<div class="project-image">
    <img src="path/to/your/image.jpg" alt="Project name">
</div>
```

Then add to CSS:
```css
.project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```

Option B: Keep placeholders but customize text
```html
<div class="placeholder-image">Your Custom Text</div>
```

### 4. Customize Colors

**In `styles.css` (lines 10-14):**

```css
--primary-color: #2c3e50;    /* Main dark color */
--accent-color: #3498db;     /* Buttons and links */
--text-dark: #2c3e50;        /* Body text */
--text-light: #7f8c8d;       /* Secondary text */
--bg-light: #f8f9fa;         /* Light backgrounds */
```

Popular professional color schemes:
- Navy & Gold: `--primary-color: #1a2332; --accent-color: #d4af37;`
- Forest & Sage: `--primary-color: #2d4739; --accent-color: #7c9a7f;`
- Burgundy & Cream: `--primary-color: #5c2e2e; --accent-color: #c17878;`

### 5. Test Locally

1. Open `index.html` in your browser (just double-click the file)
2. Check on mobile view (browser dev tools > responsive mode)
3. Test all links and modals work
4. Make sure smooth scrolling works

## Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to github.com and sign in (or create account)
2. Click "New repository"
3. Name it: `yourname.github.io` (replace yourname with your GitHub username)
4. Make it public
5. Don't add README, .gitignore, or license
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface (Easiest)**
1. Click "uploading an existing file"
2. Drag and drop: `index.html`, `styles.css`, `script.js`
3. Scroll down, add commit message: "Initial portfolio"
4. Click "Commit changes"

**Option B: Using Git (if you know Git)**
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository Settings
2. Scroll to "Pages" section (left sidebar)
3. Under "Source", select "main" branch
4. Click Save
5. Your site will be live at: `https://yourusername.github.io`

**Note:** It takes 2-5 minutes to go live the first time.

### Step 4: Add Custom Domain (Optional)

If you want `yourname.com` instead of `yourusername.github.io`:

1. Buy domain from Namecheap, Google Domains, etc. (£10-15/year)
2. In domain settings, add these DNS records:
   - A record: 185.199.108.153
   - A record: 185.199.109.153
   - A record: 185.199.110.153
   - A record: 185.199.111.153
3. In GitHub repo settings > Pages > Custom domain, enter your domain
4. Enable "Enforce HTTPS"

## Making Updates

After initial deployment, to update your site:

1. Edit files locally
2. Go to GitHub repository
3. Click on the file you want to update
4. Click pencil icon (Edit)
5. Paste new content
6. Scroll down, add commit message
7. Click "Commit changes"
8. Changes appear on your site within 1-2 minutes

## Tips

- Keep content concise - people skim websites
- Use real project examples where possible
- Test on mobile - most people will view on phones
- Get feedback before sharing widely
- Update regularly with new projects

## Troubleshooting

**Site not showing up?**
- Wait 5 minutes after first deployment
- Check repository name is exactly: `yourusername.github.io`
- Check files are in root directory (not in a folder)

**Styling looks broken?**
- Check file names are exactly: `styles.css` and `script.js`
- Check capitalization matches exactly

**Modal not opening?**
- Check modal IDs match between button and modal div
- Check script.js file loaded correctly

## Next Steps

Once deployed, you can:
- Share link on LinkedIn
- Add to CV/resume
- Use for job applications
- Send to potential clients/employers

Good luck!
