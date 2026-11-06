# Dr Ashleigh Toh — Clinical Portfolio & Oral Medicine Practice Website

This repository contains the complete, accessible, single-page static website for **Dr Ashleigh Toh**, Dental Surgeon with advanced postgraduate training in Oral Medicine.

- **Primary Deliverable:** [`index.html`](index.html) (100% self-contained: HTML5, CSS in `<style>`, JS in `<script>`, no build step or framework required).
- **Target Hosting:** GitHub Pages or Cloudflare Pages (Free tier).

---

## 1. Design & Positioning Overview

- **Audience:** Designed with equal clarity and respect for **referring dental colleagues** (initiating mucosal referrals or case discussions) and **patients/public** (educational guidance on symptoms and conditions).
- **Aesthetic Direction:** Modern professional editorial layout. Generous whitespace, refined typography, and restrained clinical authority without commercial clutter or generic stock tropes.
- **Palette D (Burgundy & Soft Blush):**
  - Primary / Headings: Deep Burgundy (`#542B39`)
  - Accent / Links: Dusty Rose (`#865365`)
  - Soft Accents / Borders: Pale Rose (`#E8DAD4`) & Muted Blush (`#C49AA2`)
  - Main Canvas: Soft White (`#FAF4F1`)
  - Card Surfaces: Pure White (`#FFFFFF`)
  - Text Contrast: High-contrast Charcoal-Burgundy (`#2C1820`), meeting WCAG 2.2 AA standards.
- **Regulatory Alignment:** Adheres to Singapore Dental Council (SDC) Ethical Code and Guidelines and Ministry of Health (MOH) regulations. Dr Toh is designated as a **Dental Surgeon** with **advanced training in Oral Medicine** (BDS Singapore, MSc Oral Medicine London).

---

## 2. Verified Practice Locations & Schedule

The website displays Dr Toh's verified locum clinics in Singapore:
1. **Teeth Q Dental Surgeons (Hougang RiverCourt)**
   - *Address:* 377 Hougang Street 32, #B1-09/10 Hougang RiverCourt, Singapore 530377
   - *Tel:* +65 6970 5715
   - *Sessions:* Sunday (9:00 AM – 6:00 PM), Wednesday (1:00 PM – 9:00 PM)
2. **Winston Tan Oral Maxillofacial Surgery (Novena)**
   - *Address:* 38 Irrawaddy Road, #11-43/44/45/46 Mount Elizabeth Novena Specialist Centre, Singapore 329563
   - *Tel:* +65 6360 0570
   - *Sessions:* Tuesday (9:00 AM – 6:00 PM), Thursday (9:00 AM – 6:00 PM)
3. **Teeth Q Dental Surgeons (Matilda Portico, Punggol)**
   - *Address:* 218 Sumang Walk, #01-02 Matilda Portico, Singapore 820218
   - *Tel:* +65 6538 2260
   - *Sessions:* Friday (9:00 AM – 6:00 PM)

*Structured data is also provided in `assets/locations.json`.*

---

## 3. Owner Action List (Before Public Launch)

Search for comments marked `OWNER PLACEHOLDER` inside `index.html` to update the following:

- [ ] **Professional Referral Email:** Replace `[DR ASHLEIGH TOH REFERRAL EMAIL TO BE ADDED]` in the `#contact` section with your preferred colleague referral email address.
- [ ] **Direct Online Booking Links (Optional):** If you or your clinics have dedicated online booking links for your sessions, you can attach them to the clinic cards in `#locations`.
- [ ] **Custom Domain (Optional):** If configuring a custom domain (e.g. `drashleightoh.com`), add a `CNAME` file or configure it in GitHub Pages / Cloudflare Pages.

---

## 4. Free Static Deployment Instructions

### Option A: GitHub Pages (Recommended)
1. Commit and push all files to your GitHub repository:
   ```bash
   git add .
   git commit -m "Build static website for Dr Ashleigh Toh"
   git push origin main
   ```
2. On GitHub, navigate to **Settings** > **Pages** (under the "Code and automation" section).
3. Under **Build and deployment**:
   - **Source:** Select `Deploy from a branch`.
   - **Branch:** Select `main` and root folder `/(root)`.
   - Click **Save**.
4. In a few minutes, your site will be live at:
   `https://whatsnottaken.github.io/dental-portfolio/`
5. *(Optional Custom Domain)* In the same Pages settings, enter your custom domain and enable **Enforce HTTPS**.

### Option B: Cloudflare Pages
1. Log into your free [Cloudflare Dashboard](https://dash.cloudflare.com/) and navigate to **Workers & Pages** > **Create application** > **Pages** > **Connect to Git**.
2. Select the `dental-portfolio` repository.
3. Configure build settings:
   - **Framework preset:** `None`
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` *(or leave blank for root)*
4. Click **Save and Deploy**. Your site will be published with global edge caching and free SSL.
