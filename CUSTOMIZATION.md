# 🎓 Customization Guide for Your Academic Website

Welcome! This guide will help you customize your GitHub Pages academic website. Follow these steps to make it your own.

---

## 📝 Quick Start: What to Update First

### 1. **_config.yaml** - Your Site Configuration

This is the **most important file** to customize first. Open [_config.yaml](_config.yaml) and update:

- **Line 2**: Replace "Your Name" with your actual name
- **Line 3**: Update the description
- **Line 4**: Change the URL to match your GitHub username
- **Lines 8-15**: Add your personal information (email, location, social media)
- **Lines 18-21**: Update your research interests
- **Line 44**: Add your logo/profile picture path

### 2. **index.md** - Your Homepage

Open [index.md](index.md) and update:

- **Lines 7-9**: Replace with your introduction
- **Lines 11-15**: Write your "About Me" section
- **Lines 17-25**: Add your Master's thesis information
- **Lines 27-30**: Add your research highlights
- **Lines 34-48**: Update your skills and expertise
- **Lines 52-58**: Add recent news/updates
- **Lines 64-71**: Update your contact information

### 3. **cv.md** - Your CV Page

Open [cv.md](cv.md) and:

- Update all sections with your actual education, research experience, etc.
- **Important**: The page links to `/assets/cv/CV_YourName.pdf` - see "Adding Your CV PDF" below

---

## 📄 Adding Your CV and Documents

### Adding Your CV (PDF)

1. **Export your CV as PDF** from Word, LaTeX, or your preferred tool
2. **Rename the file** to something like `CV_YourName.pdf` (e.g., `CV_JohnDoe.pdf`)
3. **Place it in the folder**: `/assets/cv/`
4. **Update the link** in [cv.md](cv.md):
   - Find the line: `<a href="/assets/cv/CV_YourName.pdf">`
   - Replace `CV_YourName.pdf` with your actual filename

### Adding Other Documents

**Papers/Publications**: Place PDF files in `/assets/papers/`
- Example: `/assets/papers/my_paper_2024.pdf`
- Link to them in [publications.md](publications.md)

**Presentation Slides**: Place PDF files in `/assets/slides/`
- Example: `/assets/slides/conference_2024.pdf`

**Posters**: Create `/assets/posters/` folder
- Example: `/assets/posters/poster_physics_conf_2024.pdf`

**Thesis**: Place in `/assets/papers/`
- Example: `/assets/papers/masters_thesis.pdf`

---

## 🖼️ Adding Your Profile Picture

1. **Choose a professional photo** (square format works best, e.g., 500x500px)
2. **Save it as**: `profile.jpg` or `profile.png`
3. **Place it in**: `/assets/img/`
4. **The site is already configured** to use `/assets/img/profile.jpg`
   - If you use a different filename, update line 44 in [_config.yaml](_config.yaml)

---

## 🎨 Customizing Colors and Appearance

### Change Colors

Open [assets/css/style.scss](assets/css/style.scss) and modify the color variables (lines 9-16):

```scss
:root {
  --primary-color: #2c5aa0;      /* Change this for main accent color */
  --secondary-color: #4a90e2;    /* Secondary accent */
  --link-color: #2c5aa0;         /* Link color */
  /* ... etc ... */
}
```

**Color suggestions for physics websites:**
- Academic Blue: `#2c5aa0` (default)
- Deep Purple: `#5e35b1`
- Teal/Cyan: `#00897b`
- Dark Red: `#c62828`

### Change Fonts

In [assets/css/style.scss](assets/css/style.scss), line 24, modify the `font-family`:

```scss
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, ...;
}
```

---

## 📚 Page-by-Page Customization

### research.md - Research Page

Update:
- **Lines 11-15**: Your research interests
- **Lines 21-35**: Your Master's thesis details
- **Lines 39+**: Past projects
- **Lines 61-73**: Your technical skills
- **Lines 91-95**: Future PhD directions

### publications.md - Publications

- **Lines 15+**: Add your journal articles
- **Lines 23+**: Add preprints
- **Lines 31-34**: Add your Master's thesis info
- **Lines 45+**: Add conference presentations
- **Lines 73-78**: Update citation metrics

**Format for adding a publication:**
```markdown
1. **Your Name**, Co-author. "Paper Title". *Journal Name*, Vol(Issue), pages (Year).
   - DOI: [10.xxxx/xxxxx](https://doi.org/10.xxxx/xxxxx)
   - [[PDF]](/assets/papers/paper1.pdf)
```

---

## 🔗 Adding Links

### Social Media & Academic Profiles

In [_config.yaml](_config.yaml), lines 11-15:
```yaml
linkedin: your-linkedin-username  # Just the username, not full URL
github: saulich                   # Your GitHub username
orcid: 0000-0000-0000-0000       # Your ORCID ID
google_scholar: your-scholar-id   # From your Google Scholar URL
```

### Navigation Menu

To add/remove pages from the navigation menu, edit [_config.yaml](_config.yaml), lines 24-34:

```yaml
navigation:
  - title: Home
    url: /
  - title: New Page      # Add new menu items like this
    url: /newpage
```

---

## 🚀 Publishing Your Site

### First Time Setup

1. **Go to your GitHub repository**: https://github.com/saulich/saulich.github.io
2. **Commit and push all changes**:
   ```bash
   git add .
   git commit -m "Customize academic website"
   git push
   ```
3. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
   - Click Save

4. **Wait 2-5 minutes** for the site to build
5. **Visit**: https://saulich.github.io

### Updating Your Site

After making changes:
```bash
git add .
git commit -m "Description of changes"
git push
```

Your site will automatically rebuild in a few minutes.

---

## ✅ Customization Checklist

Use this checklist to make sure you've updated everything:

- [ ] Updated personal info in `_config.yaml`
- [ ] Updated `index.md` with your introduction
- [ ] Filled out education section in `cv.md`
- [ ] Added your research interests in `research.md`
- [ ] Added your CV PDF to `/assets/cv/`
- [ ] Added profile picture to `/assets/img/`
- [ ] Updated contact information across all pages
- [ ] Customized colors in `style.scss` (optional)
- [ ] Added publications (if any) to `publications.md`
- [ ] Tested all internal links work correctly
- [ ] Committed and pushed changes to GitHub
- [ ] Verified site is live at saulich.github.io

---

## 🆘 Troubleshooting

**Site not showing up?**
- Check that GitHub Pages is enabled in repository settings
- Make sure you pushed to the correct branch (`main` or `master`)
- Wait 5-10 minutes after first push

**Images not loading?**
- Check file paths are correct (case-sensitive!)
- Make sure images are in the correct folders under `/assets/`
- Use forward slashes `/` not backslashes `\`

**Styling not applying?**
- Clear your browser cache (Cmd+Shift+R on Mac, Ctrl+Shift+R on Windows)
- Check that `style.scss` is in `/assets/css/` folder

**Links broken?**
- Internal links should be relative: `/cv` not `https://saulich.github.io/cv`
- Make sure linked files exist in the repository

---

## 📧 Need Help?

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **GitHub Pages Documentation**: https://docs.github.com/en/pages
- **Markdown Guide**: https://www.markdownguide.org/

---

## 🎯 Tips for PhD Applications

Your website can be a powerful tool for PhD applications:

1. **Keep it updated** - Add new publications, talks, and projects regularly
2. **Link it in your CV** - Add the URL prominently on your CV
3. **Share in emails** - Include it in your email signature when contacting potential advisors
4. **Be professional** - Keep content academic and professional
5. **Showcase depth** - Don't just list things, explain your contributions and impact

---

Good luck with your PhD applications! 🚀
