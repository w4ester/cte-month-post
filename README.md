# Maryland CTE Month 2026 - "Did You Know?" Social Media Toolkit

A self-service toolkit for creating and sharing branded MSDE social media posts for CTE Month and other campaigns.

## Quick Links

- **[View All Posts](index.html)** - Browse 9 "Did You Know?" posts ready for sharing
- **[Create New Post](intake.html)** - Generate a new post using the intake form

---

## How to Share Posts to Social Media (No Coding Required)

### Method 1: Copy and Paste

1. Go to the [Posts Page](index.html)
2. Find a post you want to share
3. Click the **Copy** button
4. Open your social media platform:
   - **Twitter/X** - Paste into new tweet
   - **Facebook** - Paste into new post
   - **LinkedIn** - Paste into new post
   - **Instagram** - Paste into caption (add image separately)
5. If the image doesn't paste automatically:
   - Right-click the post image on the page
   - Select "Save Image As..."
   - Attach the saved image to your social post
6. Post!

### Method 2: Download and Share

1. Click **PDF** or **DOCX** to download the post as a document
2. Open the downloaded file
3. Copy the content from the document
4. Paste into your social media platform

### Method 3: Print for Events

1. Click the **Print** button on any post
2. A print-friendly version opens with the image included
3. Print for bulletin boards, handouts, or events

---

## How to Create a New Post

### For Quick Social Media Sharing

1. Go to the [Intake Form](intake.html)
2. Fill out:
   - **Post Title** - Short title (e.g., "Work-Based Learning")
   - **Content** - Your 2-3 sentence fact
   - **Hashtags** - Check the boxes + add custom tags
   - **QR Code URL** - Link to MSDE resource page
   - **Image URL** - (Optional) Paste MSDE image URL for preview
3. Click **Generate Post**
4. Click the **Social Copy** tab
5. Click **Copy to Clipboard**
6. Paste directly into Twitter, Facebook, LinkedIn, or Instagram
7. Done! No coding needed.

### For Adding to This Toolkit (MSDE Staff)

If you want the post permanently added to the toolkit for others to share:

**Step 1: Generate the post**
- Complete the intake form
- Click "Generate Post"

**Step 2: Prepare assets**
- Save the image to the `images/` folder as `[post-id].jpg`
- Save the QR code (right-click on preview) as `images/qr-[post-id].png`

**Step 3: Add HTML to index.html**
- Copy from the "HTML" tab in the intake form
- Open `index.html` in a text editor (or request from web team)
- Paste the new `<article>` inside the posts-grid section

**Step 4: Add JavaScript data**
- Copy from the "JavaScript" tab
- Add to the `const posts = {` section in index.html

**Step 5: Update stats**
- Increment the "Posts Ready" number in the stats bar

**Step 6: Deploy**
- Save and commit changes
- New post is now available for everyone to share!

---

## For MSDE Communications Team

### Recommended Workflow

```
1. Content Creator fills out Intake Form
         ↓
2. Generate Post → Copy "Social Copy"
         ↓
3. Paste into social media platform
         ↓
4. Attach image (save from post or use MSDE photo library)
         ↓
5. Post to Twitter/Facebook/LinkedIn/Instagram
```

### To Add Posts to the Official Toolkit

Option A: **Self-Service** (if comfortable with HTML)
- Follow the "Adding to This Toolkit" steps above

Option B: **Request Addition**
- Fill out intake form
- Copy all three outputs (Social Copy, HTML, JavaScript)
- Email to web team with image attached
- Request addition to the toolkit

---

## Content Guidelines

### Writing "Did You Know?" Posts

| Element | Guideline |
|---------|-----------|
| Length | 2-3 sentences maximum |
| Opening | Start with a specific fact or number |
| Closing | End with inspiration or call-to-action |
| Punctuation | Use dashes (-) not em dashes (—) |
| Tone | Celebratory, student-focused |

### Required Hashtags

Always include:
- `#CTEMonthMD`
- `#DidYouKnow`

### Topic Hashtags

| Topic | Hashtag |
|-------|---------|
| Career clusters | `#CareerReadyMD` |
| Credentials | `#IndustryCredentials` |
| Equity/Access | `#EducationalEquity` `#AccessForAll` |
| College credits | `#DualEnrollment` `#EarlyCollege` |
| Technology | `#DigitalTechnology` `#TechCareers` |
| Healthcare | `#HealthcareCareers` |
| Student orgs | `#CTSOs` `#StudentLeadership` |

### Gradient Color Guide

| Style | Color | Use For |
|-------|-------|---------|
| Default | Red→Blue | Primary CTE topics, general facts |
| Gold | Gold→Mustard | Achievements, credentials, milestones |
| Teal | Teal→Blue | Partnerships, organizations |
| Blue | Blue gradient | Technical/professional, digital topics |

---

## What's in This Toolkit

| File | Purpose |
|------|---------|
| `index.html` | Gallery of all posts with Copy/PDF/DOCX/Print buttons |
| `intake.html` | Self-service form to create new posts |
| `images/` | Post images and QR codes |
| `README.md` | This documentation |

### Current Content

- **9 Posts** ready for sharing
- Topics covered:
  - Career Clusters & Programs
  - Industry-Recognized Credentials
  - Student Organizations (CTSOs)
  - Healthcare Pathways
  - College Credits / Dual Enrollment
  - College & Career Readiness Standard
  - Digital Technology Pathways
  - CTE Access for All (MOA)
  - 50,000+ Students Supported (MOA)

---

## Key MSDE Resources

| Topic | URL |
|-------|-----|
| CTE Programs | marylandpublicschools.org/programs/Pages/CTE/CTEprograms.aspx |
| Career Clusters | marylandpublicschools.org/programs/pages/cte/standards.aspx |
| IRCs | marylandpublicschools.org/about/pages/approved-credentials.aspx |
| CTSOs | marylandpublicschools.org/programs/pages/cte/ctso.aspx |
| Dual Enrollment | marylandpublicschools.org/about/pages/dccr/postsecondary-dual-enrollment.aspx |
| CCR Standard | marylandpublicschools.org/about/pages/dccr/meeting-ccr-standards.aspx |
| MOA Program | marylandpublicschools.org/programs/Pages/CTE/CTE%20Accountability/moa-program.aspx |

---

## Data Sources

All facts verified from:
- MSDE CTE Database
- Official MSDE website (marylandpublicschools.org)
- MD CTE Data Dashboard (mdctedata.org)

---

*Created for Maryland CTE Month 2026*
*MSDE Division of College and Career Pathways*
*w4ester & ai orchestration*
