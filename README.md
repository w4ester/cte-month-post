# CTE Month 2026 Social Media Campaign - Development Log

*Documentation of the "Side Fun" assignment: Creating MSDE-branded social media posts for CTE Month 2026*

---

## Project Summary

Created a complete social media toolkit for Maryland CTE Month 2026, including:
- 5 social media posts (4 school support + 1 "Did You Know?" submission)
- Interactive HTML demo page with official MSDE branding
- QR code generation for each post
- PDF and DOCX download capability
- Print-ready formatting

---

## Step-by-Step Process

### Step 1: Initial Content Creation (2025 Posts)

**Source:** MSDE Operations and Strategy communications

Created 4 initial posts based on real MSDE content:
1. **P-TECH Joppatowne / CECOM** - Students sworn in as federal employees
2. **Women in Maryland Construction** - 13% stat (3% above national average)
3. **National FFA Week** - Maryland FFA: 50 chapters, 2,400+ students
4. **Carver Vocational-Technical HS** - Black History Month feature (founded 1925)

**Output:** `docs/outreach/poster-cte-month.md`

---

### Step 2: 2026 Posts Update

**Source:** Real photographs and content from MSDE social media reference document

Analyzed 6 reference screenshots showing:
- Caroline Career and Technical Center - Shed building + Forklift Certifications
- Colonel Richardson High School - Biomedical program (Stop the Bleed, phlebotomy, dentistry)
- Calvert County CTE - High schoolers presenting to middle schoolers
- Harford County CTE Family Night - February 2026 event
- WCPS Youth Apprentice - SkillsUSA Maryland welding
- Student with forklift certification card

Created 5 new posts for 2026:
1. **Caroline CTC** - Construction students earning Forklift Certifications
2. **Colonel Richardson HS** - Biomedical students (Stop the Bleed, phlebotomy, dentistry)
3. **Calvert County CTE** - High schoolers advising middle schoolers
4. **Harford County CTE Family Night** - Save the Date event
5. **W4ester "Did You Know?"** - Maryland's 14 Career Clusters with 48 Programs of Study

**Output:** `docs/outreach/cte-month-2026-posts.md`

---

### Step 3: MSDE Brand Guide Discovery

**Location:** `msde-communication/BrandGuide-MSDE/MSDE-BrandGuide-2025-v1.pdf`

Extracted official brand standards:

| Element | Value |
|---------|-------|
| Primary Red | #BD0934 |
| Primary Gold | #FFC838 |
| Dark Blue | #1A4176 |
| Light Blue | #3892D4 |
| Purple | #725DA8 |
| Font | Montserrat (Google Fonts) |

**Logo files found:** `msde-communication/BrandGuide-MSDE/logo/`
- MSDE-Logo-FullColor.png
- MSDE-Logo-KnockOut.png
- MSDE-Logo-WhiteText.png

---

### Step 4: HTML Demo Page Creation

**Output:** `docs/outreach/index.html`

#### Technologies Used

| Library | Purpose | CDN Source |
|---------|---------|------------|
| QRCode.js | QR code generation | cdnjs.cloudflare.com |
| html2pdf.js | PDF export | cdnjs.cloudflare.com |
| docx.js | Word document generation | unpkg.com |
| FileSaver.js | File download handling | cdnjs.cloudflare.com |
| Google Fonts | Montserrat typography | fonts.googleapis.com |

#### Features Implemented

1. **MSDE Branding**
   - Official color palette (CSS custom properties)
   - Montserrat font family
   - Professional card-based layout

2. **Per-Post Actions**
   - Copy to clipboard (with toast notification)
   - Download as PDF
   - Download as DOCX
   - Print individual post

3. **QR Codes**
   - Auto-generated on page load
   - Links to official MSDE CTE page
   - Customized colors matching MSDE brand

4. **Responsive Design**
   - Grid layout for post cards
   - Mobile-friendly action buttons
   - Print-optimized styles

#### Code Structure

```
index.html
├── <head>
│   ├── Meta tags
│   ├── Google Fonts (Montserrat)
│   ├── External libraries (CDN)
│   └── <style> (CSS with MSDE brand variables)
├── <body>
│   ├── Header (title + subtitle)
│   ├── Posts Grid
│   │   ├── Post 1: Caroline CTC
│   │   ├── Post 2: Colonel Richardson HS
│   │   ├── Post 3: Calvert County
│   │   ├── Post 4: Harford County CTE
│   │   └── Post 5: W4ester Did You Know
│   └── Footer
└── <script>
    ├── generateQRCode()
    ├── copyPost()
    ├── downloadPDF()
    ├── downloadDOCX()
    └── printPost()
```

---

### Step 5: Security Consideration

**Issue:** Initial `printPost()` function used legacy document writing methods which triggered security hook warning for potential XSS risk.

**Solution:** Refactored to use sandboxed iframe approach with proper DOM methods, ensuring the print functionality is isolated and safe.

---

## Files Created

| File | Description |
|------|-------------|
| `docs/outreach/poster-cte-month.md` | Initial 2025 posts (markdown) |
| `docs/outreach/cte-month-2026-posts.md` | Updated 2026 posts (markdown) |
| `docs/outreach/index.html` | Interactive demo page |
| `docs/outreach/README.md` | This documentation |

---

## Post Guidelines (per MSDE)

- **Length:** 2-3 sentences maximum
- **Hashtags:** #CTEMonthMD #CareerReadyMD (primary)
- **Images:** Required - use student photos, event flyers, or infographics
- **Tone:** Celebratory, factual, student-focused
- **Source:** All facts verified from MSDE Operations and Strategy communications

---

## How to Use

### View Demo
```bash
open docs/outreach/index.html
```

### For Social Media Team
1. Open `index.html` in browser
2. Click "Copy" on desired post
3. Paste into social media platform
4. Add appropriate image from MSDE photo library

### For Print Materials
1. Click "PDF" or "DOCX" button
2. Open downloaded file
3. Print or attach to email

### For QR Code Usage
1. Right-click QR code image
2. Save image
3. Include in printed materials or slides

---

## Quality Assurance

All posts verified against:
- [x] MSDE Operations and Strategy source documents
- [x] Real photographs from Maryland schools
- [x] Official MSDE brand guide colors
- [x] 2-3 sentence length requirement
- [x] No hallucinated facts or statistics
- [x] Proper hashtag format

---

*Created: January 2026*
*Author: w4ester & ai orchestration*
