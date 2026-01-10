# AMG Invoicing Website

Professional invoicing and accounts receivable management website for AMG Invoicing, hosted on GitHub Pages.

## 🚀 Deployment Instructions

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository (e.g., `amg-invoicing-website`)
4. Choose **Public** (required for free GitHub Pages)
5. Click **Create repository**

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface**
1. In your new repository, click **uploading an existing file**
2. Drag and drop these files:
   - `index.html`
   - `styles.css`
3. Click **Commit changes**

**Option B: Using Git Command Line**
```bash
# Initialize git in this directory
git init

# Add all files
git add index.html styles.css README.md

# Commit the files
git commit -m "Initial commit: AMG Invoicing website"

# Add your GitHub repository as remote (replace USERNAME and REPO_NAME)
git remote add origin https://github.com/USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, go to **Settings**
2. Scroll down to **Pages** (in the left sidebar under "Code and automation")
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, select **main** and **/ (root)**
5. Click **Save**
6. Wait 1-2 minutes for deployment

Your site will be available at: `https://USERNAME.github.io/REPO_NAME/`

### Step 4: Set Up Formspree for Contact Form

1. Go to [Formspree.io](https://formspree.io) and sign up for a free account
2. Click **+ New Form**
3. Enter your email: `amginvoicing@gmail.com`
4. Name the form: "AMG Invoicing Contact Form"
5. Copy your form endpoint (it will look like: `https://formspree.io/f/xyzabc123`)
6. Edit `index.html` and replace `YOUR_FORM_ID` on line 180 with your actual form ID:
   ```html
   <form action="https://formspree.io/f/YOUR_ACTUAL_FORM_ID" method="POST" class="contact-form">
   ```
7. Save and push the updated file to GitHub

### Step 5: Test Your Website

1. Visit your GitHub Pages URL
2. Check all sections load correctly
3. Test the contact form by submitting a test enquiry
4. Verify you receive the email at amginvoicing@gmail.com

## 📁 File Structure

```
amg_invoicing/
├── index.html          # Main website HTML
├── styles.css          # All styling and responsive design
└── README.md          # This file with instructions
```

## 🎨 Brand Colors Used

- **Emerald Green**: `#004D24` (Primary brand color)
- **Charcoal**: `#2b2b2b` (Text and accents)
- **White**: `#ffffff` (Background and contrast)

## 📱 Features

- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Contact form with email integration
- ✅ Three service tiers with placeholder content
- ✅ SEO-friendly structure
- ✅ Modern, clean design aligned with brand guidelines
- ✅ Smooth scrolling navigation
- ✅ Industry-specific targeting for NDIS, allied health, tradies, etc.

## 🔧 Customization

### Update Service Tiers
When you finalize your pricing and service details, edit the `index.html` file starting at line 90 (Services Section).

### Change Colors
All colors are defined as CSS variables in `styles.css` at the top. Modify these to change the entire color scheme:
```css
:root {
    --emerald-green: #004D24;
    --charcoal: #2b2b2b;
    --white: #ffffff;
}
```

### Add a Logo
1. Add your logo image file to the repository
2. In `index.html`, replace the text logo (around line 20) with:
   ```html
   <img src="your-logo.png" alt="AMG Invoicing" class="logo-image">
   ```

## 📧 Contact Information

- **Email**: amginvoicing@gmail.com
- **Phone**: 0437 509 248
- **Location**: Melbourne, servicing Australia

## 🆘 Troubleshooting

**Website not showing after enabling GitHub Pages?**
- Wait 2-5 minutes for initial deployment
- Check Settings → Pages shows a green success message
- Clear your browser cache

**Contact form not working?**
- Verify you've replaced `YOUR_FORM_ID` with your actual Formspree form ID
- Check spam folder for form submissions
- Log into Formspree to see if submissions are being received

**Need to make changes?**
- Edit the files locally
- Push changes to GitHub using git or upload via web interface
- Changes will automatically deploy in 1-2 minutes

## 📄 License

© 2026 AMG Invoicing. All rights reserved.
