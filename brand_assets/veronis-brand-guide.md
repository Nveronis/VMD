# VERONIS MOBILE DETAILING — Brand & Build Guide

> **Purpose:** This document is the single source of truth for building the Veronis Mobile Detailing website. Follow every specification exactly. Do not improvise colors, fonts, spacing, or tone unless explicitly told to deviate.

---

## 1. COMPANY OVERVIEW

**Business name:** Veronis Mobile Detailing
**Type:** Mobile car detailing service (we come to the customer)
**Service area:** Worcester County, Massachusetts (towns include Worcester, Shrewsbury, Westborough, Grafton, Holden, Auburn, Millbury, Northborough, Boylston, and surrounding communities)
**Phone:** 774-200-7226
**Email:** nveronis35@gmail.com
**Facebook:** https://www.facebook.com/profile.php?id=61557473774396
**Owner:** Nicholas Veronis

**What we do:** Premium mobile car detailing — interior cleaning, exterior washing, paint correction (1-step and 2-step), ceramic coatings, and full vehicle transformations. We bring all equipment and supplies to the customer's location.

**Brand position:** Premium but accessible. We deliver luxury-level results at competitive pricing. The brand should feel high-end and professional without being pretentious or unattainable.

---

## 2. LOGO

The logo file is provided as `IMG_6622.jpg`. It features:
- A chrome/silver metallic shield shape with sharp angular edges
- Three stars at the top of the shield (signaling premium quality)
- A sports car silhouette with an orbital polisher in action
- "VERONIS MOBILE DETAILING" text with a silver-to-teal gradient
- A chrome banner element at the bottom of the shield
- Sits on a pure black background

**Logo usage rules:**
- Always display on a black or very dark background (#000000 to #0A0A0A)
- Never place the logo on a light background
- Maintain generous padding around the logo (minimum 40px on all sides)
- Do not crop, rotate, stretch, or recolor the logo
- The logo is the visual anchor of the brand — the entire site aesthetic derives from it

---

## 3. COLOR SYSTEM

The palette is extracted directly from the logo. The overall feel is **dark luxury automotive** — think high-end car showroom at night, chrome under spotlights.

### Primary Colors

| Role | Name | Hex | RGB | Usage |
|------|------|-----|-----|-------|
| Background — Primary | Midnight Black | `#000000` | 0, 0, 0 | Page backgrounds, hero sections, footer |
| Background — Elevated | Dark Surface | `#0A0A0A` | 10, 10, 10 | Cards, modals, elevated containers |
| Background — Subtle | Charcoal | `#111111` | 17, 17, 17 | Alternate section backgrounds for visual rhythm |
| Background — Card | Graphite | `#1A1A1A` | 26, 26, 26 | Service cards, pricing cards, content blocks |

### Silver / Chrome System (from logo shield and banner)

| Role | Name | Hex | RGB | Usage |
|------|------|-----|-----|-------|
| Chrome — Bright | Polished Silver | `#C0C0C0` | 192, 192, 192 | Primary headings, hero text, key UI elements |
| Chrome — Medium | Brushed Steel | `#8C8C8C` | 140, 140, 140 | Subheadings, secondary text, icon strokes |
| Chrome — Muted | Gunmetal | `#5C5C5C` | 92, 92, 92 | Tertiary text, captions, metadata, disabled states |
| Chrome — Dark | Dark Steel | `#2A2A2A` | 42, 42, 42 | Borders, dividers, subtle separators |

### Accent Color (from logo text gradient)

| Role | Name | Hex | RGB | Usage |
|------|------|-----|-----|-------|
| Accent — Primary | Steel Teal | `#4A8B9E` | 74, 139, 158 | CTA buttons, links, active states, highlights |
| Accent — Light | Frost Teal | `#6BB3C9` | 107, 179, 201 | Hover states, accent borders, subtle highlights |
| Accent — Dark | Deep Teal | `#2E6B7E` | 46, 107, 126 | Pressed/active button states, focus rings |

### Functional / Utility Colors

| Role | Name | Hex | Usage |
|------|------|-----|-------|
| Success | Chrome Green | `#4CAF50` | Confirmation states, success messages |
| Warning | Warm Amber | `#D4A843` | Warnings, limited availability notices |
| Error | Signal Red | `#D32F2F` | Error states, form validation |
| White | Pure White | `#FFFFFF` | Use VERY sparingly — only for critical contrast moments like price numbers |

### Gradient Definitions

```css
/* Chrome gradient — for decorative borders, dividers, shield-like elements */
background: linear-gradient(180deg, #C0C0C0 0%, #5C5C5C 50%, #C0C0C0 100%);

/* Teal text gradient — mirrors the logo wordmark */
background: linear-gradient(180deg, #C0C0C0 0%, #4A8B9E 100%);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;

/* Subtle surface gradient — for hero sections and key backgrounds */
background: linear-gradient(180deg, #000000 0%, #0A0A0A 50%, #111111 100%);

/* CTA button gradient */
background: linear-gradient(135deg, #4A8B9E 0%, #2E6B7E 100%);
```

### Color Rules
- **NEVER use a light/white page background.** The entire site is dark-mode only.
- Black is the dominant color (70%+ of any given screen).
- Silver/chrome tones handle all text hierarchy.
- Teal is the ONLY color accent — use it for interactive elements and sparingly for visual emphasis. Do not introduce additional accent colors.
- Avoid pure white (#FFFFFF) for body text. Use Polished Silver (#C0C0C0) for headings and Brushed Steel (#8C8C8C) for body copy.
- All images should sit naturally against dark backgrounds. Add subtle dark overlays to photos if needed.

---

## 4. TYPOGRAPHY

### Font Stack

| Role | Font | Fallback | Weight | Usage |
|------|------|----------|--------|-------|
| Headings | **Montserrat** | Arial, sans-serif | 600 (Semi-Bold), 700 (Bold) | All headings H1–H6 |
| Body | **Inter** | Helvetica, Arial, sans-serif | 400 (Regular), 500 (Medium) | Paragraph text, descriptions, form labels |
| Accent / UI | **Montserrat** | Arial, sans-serif | 500 (Medium) | Buttons, navigation links, badges, labels |
| Monospace | **JetBrains Mono** | Courier New, monospace | 400 | Pricing numbers, phone number (optional stylistic choice) |

### Type Scale

| Element | Size (desktop) | Size (mobile) | Weight | Color | Letter Spacing | Line Height | Text Transform |
|---------|---------------|---------------|--------|-------|----------------|-------------|----------------|
| H1 — Hero | 64px | 36px | 700 | #C0C0C0 | -0.02em | 1.1 | Uppercase |
| H2 — Section | 40px | 28px | 700 | #C0C0C0 | -0.01em | 1.2 | None |
| H3 — Card Title | 24px | 20px | 600 | #C0C0C0 | 0 | 1.3 | None |
| H4 — Label | 18px | 16px | 600 | #8C8C8C | 0.05em | 1.4 | Uppercase |
| Body — Large | 18px | 16px | 400 | #8C8C8C | 0 | 1.7 | None |
| Body — Regular | 16px | 15px | 400 | #8C8C8C | 0 | 1.6 | None |
| Body — Small | 14px | 13px | 400 | #5C5C5C | 0 | 1.5 | None |
| Caption | 12px | 11px | 400 | #5C5C5C | 0.03em | 1.4 | None |
| Button | 16px | 15px | 500 | #FFFFFF | 0.05em | 1.0 | Uppercase |
| Nav Link | 14px | 14px | 500 | #8C8C8C | 0.08em | 1.0 | Uppercase |
| Price | 32px | 24px | 700 | #FFFFFF | -0.01em | 1.0 | None |

### Typography Rules
- Headings use Montserrat; body uses Inter. Do not swap them.
- H1 hero text can optionally use the teal gradient (silver-to-teal) for visual impact.
- Keep line lengths under 70 characters for readability on wide screens.
- Use letter-spacing on uppercase elements for breathing room.

---

## 5. SPACING & LAYOUT

### Spacing Scale (8px base unit)

| Token | Value | Usage |
|-------|-------|-------|
| `xs` | 4px | Tight internal padding, icon gaps |
| `sm` | 8px | Between related elements (label to input) |
| `md` | 16px | Default component internal padding |
| `lg` | 24px | Between components within a section |
| `xl` | 32px | Section internal padding |
| `2xl` | 48px | Between major sections |
| `3xl` | 64px | Hero section padding, major visual breaks |
| `4xl` | 96px | Top-level section separation (desktop) |

### Layout Grid

| Property | Desktop | Tablet | Mobile |
|----------|---------|--------|--------|
| Max content width | 1200px | 100% | 100% |
| Column grid | 12 columns | 8 columns | 4 columns |
| Gutter | 24px | 20px | 16px |
| Page margin (sides) | auto-centered | 32px | 16px |
| Section vertical padding | 96px top/bottom | 64px | 48px |

### Breakpoints

| Name | Value | Description |
|------|-------|-------------|
| Mobile | 0–639px | Single column, stacked layout |
| Tablet | 640–1023px | Two-column where appropriate |
| Desktop | 1024–1439px | Full multi-column layout |
| Wide | 1440px+ | Centered content, max-width enforced |

---

## 6. UI COMPONENTS

### Borders & Corners

**CRITICAL: All corners are sharp. Border-radius is 0px across the entire site.** This is a hard brand rule that matches the angular shield in the logo. No rounded corners on anything — buttons, cards, images, inputs, modals, nothing.

```css
border-radius: 0;
```

The only exception: fully circular elements like avatar placeholders or loading spinners.

### Buttons

**Primary CTA:**
```css
background: linear-gradient(135deg, #4A8B9E 0%, #2E6B7E 100%);
color: #FFFFFF;
padding: 14px 32px;
font-family: 'Montserrat', sans-serif;
font-size: 16px;
font-weight: 500;
letter-spacing: 0.05em;
text-transform: uppercase;
border: none;
border-radius: 0;
cursor: pointer;
transition: all 0.3s ease;
```

**Primary CTA Hover:**
```css
background: linear-gradient(135deg, #6BB3C9 0%, #4A8B9E 100%);
transform: translateY(-1px);
box-shadow: 0 4px 20px rgba(74, 139, 158, 0.3);
```

**Secondary / Ghost Button:**
```css
background: transparent;
color: #C0C0C0;
padding: 14px 32px;
border: 1px solid #5C5C5C;
font-family: 'Montserrat', sans-serif;
font-size: 16px;
font-weight: 500;
letter-spacing: 0.05em;
text-transform: uppercase;
border-radius: 0;
transition: all 0.3s ease;
```

**Ghost Hover:**
```css
border-color: #4A8B9E;
color: #4A8B9E;
```

### Cards (Service / Pricing)

```css
background: #1A1A1A;
border: 1px solid #2A2A2A;
border-radius: 0;
padding: 32px;
transition: all 0.3s ease;
```

**Card Hover:**
```css
border-color: #4A8B9E;
box-shadow: 0 0 30px rgba(74, 139, 158, 0.08);
transform: translateY(-2px);
```

**Featured / Premium Card (e.g., Diamond Detail):**
```css
border-color: #4A8B9E;
box-shadow: 0 0 40px rgba(74, 139, 158, 0.12);
/* Add a subtle top accent border */
border-top: 2px solid #4A8B9E;
```

### Navigation Bar

```css
background: rgba(0, 0, 0, 0.85);
backdrop-filter: blur(20px);
-webkit-backdrop-filter: blur(20px);
border-bottom: 1px solid #2A2A2A;
padding: 16px 0;
position: fixed;
top: 0;
width: 100%;
z-index: 1000;
```

### Form Inputs

```css
background: #111111;
border: 1px solid #2A2A2A;
border-radius: 0;
color: #C0C0C0;
padding: 14px 16px;
font-family: 'Inter', sans-serif;
font-size: 16px;
transition: border-color 0.3s ease;
```

**Input Focus:**
```css
border-color: #4A8B9E;
outline: none;
box-shadow: 0 0 0 2px rgba(74, 139, 158, 0.15);
```

### Dividers / Section Separators

```css
/* Standard divider */
border-top: 1px solid #2A2A2A;

/* Accent divider (use sparingly, e.g., below hero) */
height: 2px;
background: linear-gradient(90deg, transparent 0%, #4A8B9E 50%, transparent 100%);
```

---

## 7. PAGE STRUCTURE & SECTIONS

Build the site as a **single-page scrolling website** with a sticky nav that links to anchored sections. Include these sections in this order:

### 7.1 Navigation (sticky top)
- Logo (left)
- Links: Home | Services | Gallery | About | Contact (center or right)
- CTA button: "Get A Quote" (far right, primary teal button)
- Mobile: hamburger menu with slide-out panel (dark background)

### 7.2 Hero Section
- Full-viewport height (100vh)
- Dark background with a subtle radial gradient or a high-quality car image with a dark overlay (70–80% black overlay)
- Headline: large, bold, H1 — something specific and benefit-driven (NOT generic "Professional Mobile Detailing")
  - Suggested: "PREMIUM DETAILING. AT YOUR DOOR." or "SHOWROOM RESULTS. YOUR DRIVEWAY."
- Subheadline: one line describing the value prop for Worcester County
  - Suggested: "Worcester County's trusted mobile detailing — we bring the shine to you."
- Two CTAs side by side: "Get A Quote" (primary teal) + "Call Now" (ghost/secondary)
- Phone number visible in hero area

### 7.3 Services Section
- Section heading: "Our Services"
- Three-column card layout (stacks on mobile):
  - **Complete Details** (Silver / Gold / Diamond packages)
  - **Interior Only** (Basic Interior / Deep Clean Interior)
  - **Exterior Only** (Basic Wash / Deep Clean Exterior / Paint Correction / Ceramic Coating)
- Each card: icon or small image, title, brief description, "View Pricing" link
- Below the overview cards, expandable or scrollable **detailed pricing breakdowns** for each package showing:
  - Package name
  - Price range (e.g., "$150–$185")
  - What's included (bulleted feature list)
- Highlight the Diamond Detail or most popular package with a "MOST POPULAR" badge and the accent border treatment

### 7.4 Gallery / Our Work Section
- Section heading: "Our Work" or "Transformations"
- **Before & After pairs** are the priority format — side by side or with a slider
- If before/after is not available, use a clean masonry or grid gallery
- Minimum 6 images, ideally 9–12
- Lightbox on click for full-size viewing
- Captions optional (vehicle type + service performed)

### 7.5 About Section
- Section heading: "About Veronis Mobile Detailing"
- Focus on experience, number of vehicles detailed, commitment to quality, and equipment
- **Do NOT mention student status** — lead with expertise and passion for automotive care
- Include a professional photo of the owner or the operation (van/setup/working on a car)
- Keep it to 2–3 short paragraphs maximum

### 7.6 Testimonials Section
- Section heading: "What Our Customers Say"
- Display 3–5 testimonials (pull from Google and Facebook reviews)
- Include customer name and star rating
- If only one testimonial is available, display it prominently as a featured quote with large text

### 7.7 Service Area Section
- Section heading: "Areas We Serve"
- List major towns: Worcester, Shrewsbury, Westborough, Grafton, Holden, Auburn, Millbury, Northborough, Boylston, and surrounding communities
- Optional: embedded map or simple styled list
- Note: "Don't see your town? Contact us — we likely cover your area."

### 7.8 FAQ Section
- Section heading: "Frequently Asked Questions"
- Accordion-style expand/collapse
- Minimum questions to include:
  - "How long does a detail take?"
  - "Do I need to provide water or electricity?"
  - "What if it rains on my appointment day?"
  - "What areas do you serve?"
  - "How do I prepare my vehicle?"
  - "Do you offer ceramic coating?"
  - "What products do you use?"

### 7.9 Contact / Quote Section
- Section heading: "Get Your Free Quote"
- Contact form with fields: First Name, Last Name, Phone, Email, Vehicle Year/Make/Model, Service Interested In (dropdown), Preferred Date, Additional Notes
- Display phone number and email alongside the form
- Social media links (Facebook, Instagram)

### 7.10 Footer
- Logo (smaller)
- Quick nav links
- Contact info (phone, email)
- Social media icons
- Service area summary (one line)
- Copyright: "© 2025 Veronis Mobile Detailing. All rights reserved."
- "Serving Worcester County, MA"

---

## 8. SERVICE & PRICING DATA

Use these exact packages and prices throughout the site:

### Complete Details
| Package | Price | Interior Includes | Exterior Includes |
|---------|-------|-------------------|-------------------|
| Silver Detail | $150–$185 | Dust/dirt/grime removal, full vacuum, window cleaning, odor remover | Door jamb cleaning, rims/tires/wheels cleaned, foam spray wash, hand scrub wash |
| Gold Detail | $205–$245 | Everything in Silver + shampooing seats/mats/floors, leather conditioning | Everything in Silver + exterior paint protection, wheel & tire protection |
| Diamond Detail | $250–$295 | Everything in Gold + protection to all plastics and vinyl | Everything in Gold + clay bar treatment, ceramic wax, trim restoration & protection |

### Interior Only
| Package | Price | Includes |
|---------|-------|----------|
| Basic Interior | $105–$125 | Dust/dirt/grime removal, full vacuum, window cleaning, odor remover |
| Deep Clean Interior | $130–$160 | Everything in Basic + shampooing seats/mats/floors, leather conditioning, plastic & vinyl protection |

### Exterior Only & Paint Correction
| Package | Price | Includes |
|---------|-------|----------|
| Basic Wash | $100–$150 | Foam spray wash, hand scrub wash, tire/wheel/rim cleaning. Optional wax or clay bar for additional charge |
| 1-Step Paint Correction | $315–$350 | Full wash, clay bar decontamination, paint prep, one-stage machine polish. Optional ceramic coating add-on |
| 2-Step Paint Correction | $415–$450 | Full wash, clay bar, paint prep, two-stage compound and polish. Optional ceramic coating add-on |

### Add-On (feature separately)
| Service | Price | Description |
|---------|-------|-------------|
| Ceramic Coating | TBD / Quote | Professional-grade ceramic coating for long-term paint protection. Applied after paint correction for best results. |

---

## 9. MOTION & ANIMATION

Keep animations subtle, smooth, and premium-feeling. Nothing flashy or distracting.

| Element | Animation | Duration | Easing |
|---------|-----------|----------|--------|
| Page sections on scroll | Fade up + slight translateY(20px → 0) | 600ms | ease-out |
| Cards on hover | Lift (translateY -2px) + border glow | 300ms | ease |
| Buttons on hover | Subtle lift + shadow expansion | 300ms | ease |
| Navigation on scroll | Background blur intensifies | 200ms | ease |
| Gallery images | Scale(1 → 1.03) on hover | 400ms | ease |
| Stat counters (if used) | Count-up animation on scroll into view | 2000ms | ease-out |

**Rules:**
- No bounce effects
- No spinning or rotating animations
- No parallax scrolling (keep it clean and fast)
- Prefer opacity + transform animations for performance (GPU-accelerated)
- Respect `prefers-reduced-motion` media query — disable all animations for users who request it

---

## 10. IMAGERY GUIDELINES

- **Prioritize real photos** of actual Veronis work over stock photography
- All photos should be high resolution and well-lit
- Apply dark overlays (50–80% black) when using photos as section backgrounds
- Before/after pairs are the highest-value visual content — prioritize these
- Acceptable stock photo subjects if needed: close-up of paint correction, foam wash in progress, ceramic coating application, luxury car details (grilles, wheels, paint reflections)
- Avoid cheesy stock photos of people smiling at cameras in a garage

---

## 11. VOICE & COPY GUIDELINES

### Tone
- **Confident** — we know what we're doing, no hedging
- **Direct** — short sentences, clear language, no filler
- **Premium but approachable** — professional without being stuffy
- **Worcester County local** — we're your neighbor, not a faceless corporation

### Copy Rules
- Lead with benefits, not features ("Restore your paint's showroom shine" not "We use DA polishers")
- Use "your" and "you" frequently — make it about the customer
- Avoid overused detailing clichés: "where convenience meets quality," "fresh-off-the-lot," "one-stop shop"
- Keep paragraphs short (2–3 sentences max)
- Every section should have a clear CTA or next step
- Service descriptions should focus on the outcome/result, not just the process

### Sample Headlines
- Hero: "SHOWROOM RESULTS. YOUR DRIVEWAY."
- Services: "Choose Your Detail"
- Gallery: "See The Difference"
- About: "Built On Passion. Driven By Results."
- Testimonials: "Don't Take Our Word For It"
- Contact: "Ready For That New-Car Feel?"

---

## 12. SEO & META

### Page Title
`Veronis Mobile Detailing | Premium Car Detailing in Worcester County, MA`

### Meta Description
`Professional mobile car detailing serving Worcester County, MA. Interior & exterior detailing, paint correction, and ceramic coating — brought to your door. Get a free quote today.`

### Target Keywords (use naturally in copy)
- mobile detailing Worcester MA
- car detailing Worcester County
- paint correction Worcester MA
- ceramic coating Worcester Massachusetts
- mobile car wash Shrewsbury MA
- auto detailing near me Worcester
- interior car detailing Central Massachusetts

### Schema Markup
Include LocalBusiness structured data:
```json
{
  "@context": "https://schema.org",
  "@type": "AutoRepair",
  "name": "Veronis Mobile Detailing",
  "telephone": "774-200-7226",
  "email": "nveronis35@gmail.com",
  "url": "https://www.veronismobiledetailing.com",
  "areaServed": {
    "@type": "AdministrativeArea",
    "name": "Worcester County, Massachusetts"
  },
  "serviceType": ["Car Detailing", "Paint Correction", "Ceramic Coating", "Mobile Detailing"],
  "priceRange": "$100-$450"
}
```

---

## 13. TECHNICAL REQUIREMENTS

- **Mobile-first responsive design** — must look perfect on phones first, then scale up
- **Fast loading** — optimize all images (WebP format preferred, lazy loading below the fold)
- **Accessible** — proper heading hierarchy, alt text on all images, sufficient color contrast, keyboard navigable
- **Smooth scrolling** between sections via nav links
- **Contact form** must validate fields and provide clear success/error feedback
- **Sticky navigation** that is transparent over the hero then gains a dark background on scroll
- Use semantic HTML5 elements (header, nav, main, section, footer)
- Include Open Graph meta tags for social sharing

---

## 14. CLAUDE CODE QUICK REFERENCE

When building this site, follow these priorities:

1. **Dark theme is non-negotiable.** Every background is black/near-black. No white pages, no light sections.
2. **Sharp corners everywhere.** `border-radius: 0` on all elements. This is the brand signature.
3. **Teal is the only accent.** Do not introduce blue, purple, red, or any other accent color.
4. **Silver text hierarchy.** Bright silver for headings → medium silver for body → dark silver for captions.
5. **The logo is provided as an image file.** Display it in the nav and footer. Do not attempt to recreate it in CSS/SVG.
6. **Montserrat for headings, Inter for body.** Import from Google Fonts.
7. **Mobile-first.** Build the mobile layout first, then add desktop breakpoints.
8. **Real content.** Use the exact pricing, service descriptions, and business information from this guide. Do not generate placeholder text.
9. **Performance matters.** Lazy load images, use WebP, minimize JavaScript.
10. **Worcester County, MA** is the service area. Not Amherst. Not Pioneer Valley. Not Boston.
