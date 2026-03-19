# RM Nirman Buildcon Pvt Ltd — Official Website

> *"We don't just build structures — we build trust, one project at a time."*

![Version](https://img.shields.io/badge/version-1.0.0-gold)
![Status](https://img.shields.io/badge/status-live-brightgreen)
![Language](https://img.shields.io/badge/language-HTML%20%7C%20CSS%20%7C%20JS-orange)
![Founded](https://img.shields.io/badge/founded-2008-blue)
![License](https://img.shields.io/badge/license-Private-red)

---

## 📌 About This Project

This is the official website for **RM Nirman Buildcon Pvt Ltd** — a construction and infrastructure company founded in 2008 by **Ram Iqbal**, operating across **Delhi, Noida, Bihar, and Himachal Pradesh** with 100+ skilled workers.

The website is built as a **single-file HTML application** — no frameworks, no dependencies, no build tools required. Just open in a browser and it works.

---

## 🌐 Live Preview

```
Open: rmnirman_website.html
```

---

## ✨ Features

| Feature | Description |
|---|---|
| 🌙☀️ **Day / Night Mode** | Smooth toggle between dark gold theme and warm cream theme. Preference saved in localStorage |
| 🌐 **3 Language Support** | Switch between English, Hindi (हिंदी), and Hinglish with one click |
| 📱 **Fully Responsive** | Works on mobile, tablet, and desktop |
| ⚡ **No Dependencies** | Pure HTML, CSS, JavaScript — no npm, no build step |
| 🎨 **Premium Design** | Dark gold luxury aesthetic with smooth animations |
| 🔗 **Single File** | Entire website in one `.html` file — easy to host anywhere |

---

## 📁 Project Structure

```
rm-nirman-buildcon/
│
├── rmnirman_website.html      ← Main website (single file)
├── README.md                  ← This file
│
└── assets/                    ← (Optional) Add your own images here
    ├── logo.png
    ├── projects/
    │   ├── project1.jpg
    │   └── project2.jpg
    └── team/
        ├── niraj.jpg
        └── arun.jpg
```

---

## 🏗️ Sections

The website includes the following sections:

1. **Hero** — Full-screen banner with company tagline and key stats
2. **Services** — 6 service cards (Residential, Commercial, Infrastructure, Renovation, Design, PM)
3. **About Us** — Company story with founder information and key features
4. **Team** — Ram Iqbal (Founder), Niraj (Director), Arun (Director)
5. **Projects Portfolio** — 5 featured project cards with hover effects
6. **Why Choose Us** — 4 key differentiators + stats box
7. **Contact** — Contact details + inquiry form
8. **Footer** — Links, branding, and copyright

---

## 🚀 Getting Started

### Option 1 — Open Directly
```bash
# Just open the file in any browser
open rmnirman_website.html
```

### Option 2 — Local Server (Recommended)
```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .

# Then open: http://localhost:8000/rmnirman_website.html
```

### Option 3 — Deploy to Hosting
Upload `rmnirman_website.html` to any hosting provider:
- **Hostinger** — Recommended for India (₹3,000/year)
- **GoDaddy** — Good domain + hosting combo
- **Netlify** — Free tier available, drag & drop deploy
- **GitHub Pages** — Free, rename file to `index.html`

---

## ⚙️ Customization Guide

### Update Contact Information
Search for and replace these placeholders in the HTML file:

```
+91 87009 47487    →    Your actual phone number
info@rmnirman.com  →    Your actual email address
Delhi, India       →    Your actual office address
```

### Update Stats / Numbers
Search for these values and update them:

```html
<!-- Hero Stats -->
17+   → Years of experience
100+  → Number of workers
4     → Number of states

<!-- Why Us Box -->
95%   → Client satisfaction rate
2008  → Founded year
```

### Add Real Project Photos
Replace Unsplash image URLs with your own:

```html
<!-- Find lines like this: -->
src="https://images.unsplash.com/photo-XXXXX"

<!-- Replace with your own image: -->
src="assets/projects/your-project.jpg"
```

### Change Colors
All colors are defined as CSS variables at the top of the `<style>` block:

```css
:root {
  --gold:       #C9972B;   /* Primary gold accent */
  --gold-light: #E8B84B;   /* Lighter gold for hover */
  --dark:       #0D0D0D;   /* Main background (night) */
  --dark2:      #161616;   /* Section background */
  --dark3:      #1E1E1E;   /* Card background */
  --white:      #F5F2ED;   /* Text color */
  --gray:       #8A8A8A;   /* Muted text */
}
```

---

## 🌐 Language System

The website supports 3 languages via `data-*` attributes:

```html
<!-- Example element with all 3 languages -->
<h2 class="section-title"
  data-en="We Build Everything"
  data-hi="हम सब कुछ बनाते हैं"
  data-hl="Har Cheez Banate Hain Hum">
  We Build Everything
</h2>
```

To add or update translations, find the relevant element and update its `data-hi` (Hindi) or `data-hl` (Hinglish) attribute.

---

## 🌙 Day / Night Mode

The theme is controlled by adding/removing the `day-mode` class on the `<html>` element:

```javascript
// Toggle theme
function toggleTheme() {
  const isDay = document.documentElement.classList.toggle('day-mode');
  localStorage.setItem('rmtheme', isDay ? 'day' : 'night');
}
```

Night mode CSS variables (default):
```css
:root {
  --dark: #0D0D0D;
  --white: #F5F2ED;
}
```

Day mode CSS variables (`.day-mode` class):
```css
html.day-mode {
  --dark: #F7F4EE;
  --white: #1A1A1A;
}
```

---

## 🏢 Company Information

| Field | Details |
|---|---|
| **Company Name** | RM Nirman Buildcon Pvt Ltd |
| **Founded** | 2008 |
| **Founder** | Ram Iqbal |
| **Directors** | Niraj, Arun |
| **Workforce** | 100+ Skilled Workers |
| **Operations** | Delhi, Noida, Bihar, Himachal Pradesh |
| **Services** | Residential, Commercial, Infrastructure, Renovation |
| **Website** | rmnirman.com *(recommended domain)* |
| **Email** | info@rmnirman.com *(to be set up)* |

---

## 📋 To-Do / Next Steps

- [ ] Purchase domain — `rmnirman.com` or `rmnirmanbuildcon.com`
- [ ] Set up hosting (Hostinger / GoDaddy / Netlify)
- [ ] Replace placeholder phone number with real number
- [ ] Replace placeholder email with real business email
- [ ] Add real office address in contact section
- [ ] Upload actual project photos to `assets/projects/`
- [ ] Add team photos for Niraj and Arun
- [ ] Set up Google Maps embed for office location
- [ ] Connect contact form to email (using Formspree or similar)
- [ ] Register company on Google My Business
- [ ] Submit website to GeM Portal and PWD portals

---

## 🔧 Tech Stack

| Technology | Usage |
|---|---|
| **HTML5** | Structure and content |
| **CSS3** | Styling, animations, day/night mode |
| **Vanilla JavaScript** | Language switcher, theme toggle |
| **Google Fonts** | Playfair Display + Barlow typefaces |
| **Unsplash** | Placeholder project images (replace with real ones) |

---

## 📞 Contact

For website-related queries:

- **Email:** info@rmnirman.com
- **Phone:** +91 87009 47487
- **Office:** Delhi, India
- **Working Hours:** Monday – Saturday, 9AM to 7PM

---

## 📄 License

This website and its code are the **private property of RM Nirman Buildcon Pvt Ltd**.
Unauthorized copying, distribution, or use is strictly prohibited.

© 2008–2025 RM Nirman Buildcon Pvt Ltd. All Rights Reserved.
Founded by **Ram Iqbal**.

---

<p align="center">
  Built with ♥ in Delhi, India &nbsp;|&nbsp; RM Nirman Buildcon Pvt Ltd
</p>
