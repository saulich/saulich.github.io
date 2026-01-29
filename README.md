# Academic Portfolio Website

A professional GitHub Pages website for physics graduate students and researchers.

## 🌐 Live Site

Visit: [https://saulich.github.io](https://saulich.github.io)

## 📋 Features

- **Professional Homepage** - Introduce yourself and your research
- **Research Page** - Showcase your projects and technical skills
- **Publications** - List papers, presentations, and thesis work
- **CV Page** - Online CV with PDF download option
- **Customizable Design** - Easy color and style customization
- **Responsive** - Works on desktop and mobile devices

## 🚀 Quick Start

1. **Customize your site** - Follow the detailed instructions in [CUSTOMIZATION.md](CUSTOMIZATION.md)
2. **Add your information** - Update all files with your personal details
3. **Add your CV** - Place your CV PDF in `/assets/cv/`
4. **Push to GitHub** - Your site will be live at `https://[username].github.io`

## 📁 Site Structure

```
saulich.github.io/
├── _config.yaml           # Site configuration (START HERE!)
├── index.md               # Homepage
├── research.md            # Research & projects page
├── publications.md        # Publications & presentations
├── cv.md                  # CV page
├── CUSTOMIZATION.md       # Detailed customization guide
├── README.md             # This file
└── assets/
    ├── css/
    │   └── style.scss    # Custom styling
    ├── cv/               # Place your CV PDF here
    ├── papers/           # Place paper PDFs here
    ├── slides/           # Place presentation slides here
    └── img/              # Place images here (profile photo, etc.)
```

## 📝 Where to Add Your Files

### Your CV (PDF)
- **Location**: `/assets/cv/CV_YourName.pdf`
- **Update**: Link in [cv.md](cv.md) (line 9)

### Profile Picture
- **Location**: `/assets/img/profile.jpg` (or `.png`)
- **Update**: Path in [_config.yaml](_config.yaml) (line 44)

### Papers & Publications
- **Location**: `/assets/papers/`
- **Link from**: [publications.md](publications.md)

### Presentation Slides
- **Location**: `/assets/slides/`
- **Link from**: [publications.md](publications.md)

## 🎨 Customization

All customization instructions are in [CUSTOMIZATION.md](CUSTOMIZATION.md). Key areas:

- **Personal info**: Edit [_config.yaml](_config.yaml)
- **Colors & fonts**: Edit [assets/css/style.scss](assets/css/style.scss)
- **Content**: Edit the `.md` files for each page

## 🛠️ Built With

- **Jekyll** - Static site generator
- **GitHub Pages** - Free hosting
- **Minimal Theme** - Clean, academic design

## 📧 Questions?

See [CUSTOMIZATION.md](CUSTOMIZATION.md) for detailed instructions and troubleshooting.

---

**Good luck with your PhD applications!** 🎓