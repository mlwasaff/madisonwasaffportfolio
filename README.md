# Madison Wasaff Portfolio — Setup Guide

## Folder Structure
```
portfolio/
├── index.html          ← Homepage
├── about.html          ← About page
├── ux-design.html      ← UX Design page
├── art.html            ← Art page (Photography, 3D, Printmaking)
├── digital-design.html ← Digital Design / SMAD page
├── style.css           ← All custom styles (do not delete)
├── images/             ← PUT ALL YOUR IMAGES HERE
│   ├── hero-photo.jpg
│   ├── headshot.jpg
│   ├── work-photography.jpg
│   ├── work-ux.jpg
│   ├── work-3d.jpg
│   ├── work-digital.jpg
│   ├── photo-1.jpg ... photo-6.jpg   (Photography gallery)
│   ├── 3d-1.jpg ... 3d-6.jpg         (3D Design gallery)
│   ├── print-1.jpg ... print-4.jpg   (Printmaking gallery)
│   ├── ux-research-1.jpg, ux-research-2.jpg
│   ├── ux-narrative-1.jpg ... ux-narrative-3.jpg
│   ├── ux-ia-1.jpg, ux-ia-2.jpg
│   ├── digital-featured.jpg
│   └── digital-1.jpg ... digital-5.jpg
└── documents/          ← PUT ALL YOUR PDFs HERE
    ├── madison-wasaff-resume.pdf
    ├── research-project-1.pdf
    ├── research-project-2.pdf
    ├── narrative-1.pdf ... narrative-3.pdf
    ├── ia-project-1.pdf, ia-project-2.pdf
    ├── digital-featured.pdf
    └── digital-1.pdf ... digital-5.pdf
```

---

## Quickstart: Replace YOUR info

### 1. Add Images
Create an `images/` folder in the same directory as your HTML files.
Drop your photos in with the filenames listed above.
(You can rename your files to match, or find & replace the filenames in the HTML.)

### 2. Add Documents
Create a `documents/` folder.
Place your PDF files in it using the names listed above.

### 3. Update Personal Info (find & replace in each file)
- `youremail@email.com` → your real email
- Social links: find `href="#"` near Instagram/LinkedIn icons → replace with your profile URLs
- Name "Madison Wasaff" → your own name (if personalizing)

### 4. Add Gallery Images
Each gallery section has clearly labeled image slots like:
```html
<!-- images/photo-1.jpg -->
<img src="images/photo-1.jpg" alt="Photo 1">
```
Simply add more `<div class="gallery-item">` blocks by copying an existing one.

### 5. Add Project Cards
Each project card has a template comment above it. Copy a card block
and update the image, tag, title, description, and document link.

---

## Editing Tips

### Change the hero photo (index.html, line ~72)
```html
<img src="images/hero-photo.jpg" alt="Madison Wasaff">
```

### Change section text
All editable text sections have a comment like:
```html
<!--
  ══════════════════════════════════════
  PERSONAL BIO — edit this paragraph
  ══════════════════════════════════════
-->
```

### Change colors (style.css, top of file)
```css
--pink:       #d4a0a0;   ← adjust pink tone
--green:      #8aaa8a;   ← adjust green tone
--cream:      #f5f2ee;   ← background warmth
--charcoal:   #2e2b28;   ← dark text color
```

### Add more pages
1. Copy `digital-design.html` as a template
2. Update the `<title>`, nav `active` class, and content
3. Link to it from the nav in all other pages

---

## File Requirements
- Bootstrap 5.3.8 is loaded from CDN (requires internet)
- Google Fonts (Cormorant Garamond + DM Sans) loaded from CDN
- No JavaScript frameworks — only vanilla JS + Bootstrap
- All images should be JPEG or PNG
- Recommended image sizes:
  - Hero photo: 800×1060px (portrait)
  - Headshot: 600×800px (portrait)
  - Work cards: 800×600px (landscape)
  - Gallery images: any size (auto-fits)
  - Project images: 1200×675px (16:9)
