================================================================
  LIMBURG GERMAN CULTURAL CENTER — WEBSITE README
  ================================================================
  Version:  1.0
  Created:  2026
  Author:   Ninga Abbo Xavier / Culture Splendours
  Contact:  info@limburggermanculturalcenter.cm
================================================================

FOLDER STRUCTURE
────────────────
limburg-website/
│
├── index.html                    ← HOMEPAGE  (open this in browser)
│
├── pages/
│   ├── german-language.html      ← German Language School + Registration + Student Portal
│   ├── services.html             ← All 8 services
│   ├── about.html                ← About, History, Team, Partners
│   ├── heritage.html             ← Heritage & Tourism, Tour packages
│   ├── news.html                 ← News, Events, Newsletter
│   └── contact.html              ← Contact form, Map, WhatsApp
│
├── assets/
│   ├── css/
│   │   └── shared.css            ← Shared styles (nav, footer, buttons)
│   ├── js/                       ← Place any extra JS files here
│   ├── fonts/                    ← Place custom fonts here (if any)
│   ├── videos/                   ← Place MP4 videos here
│   └── images/
│       ├── hero/                 ← Hero background photos
│       ├── services/             ← Service section photos
│       ├── about/                ← About page photos & partner logos
│       ├── team/                 ← Team member portrait photos
│       ├── tourism/              ← Tour & heritage photos
│       ├── news/                 ← News article thumbnails
│       └── gallery/              ← Photo Gallery exhibition images
│
├── IMAGE_REFERENCE.txt           ← Full guide to all image slots
└── README.txt                    ← This file

================================================================
HOW TO USE THIS WEBSITE
================================================================

1. OPEN IN BROWSER
   Double-click index.html to open the homepage in any browser.
   All pages link to each other — no server needed for browsing.

2. EDIT TEXT CONTENT
   Open any .html file in a text editor (Notepad, VS Code, etc.)
   Search for <!-- TO EDIT: --> comments — they mark every
   section of text that should be customized.

3. ADD IMAGES
   See IMAGE_REFERENCE.txt for the full list of all image slots.
   Short version:
   - Save building photo as: assets/images/hero/building.jpg
   - Uncomment background-image in each page's <style> block
   - Replace placeholder <div> blocks with <img> tags

4. ADD THE BUILDING HERO PHOTO (most important step)
   Every page has this comment in its <style> block:
     /* background-image: url('../assets/images/hero/building.jpg'); */
   Step 1: Save your building photo to assets/images/hero/building.jpg
   Step 2: Remove the /* and */ from that line in each page
   The dark overlay already makes ALL text visible on any photo.

5. UPDATE CONTACT DETAILS
   Search for these values across all pages and update them:
   - Phone:   +237 678 001 127
   - Email:   info@limburggermanculturalcenter.cm
   - Address: Isokolo, adjacent to the market, Limbe

6. CONNECT THE CONTACT FORM
   In pages/contact.html, find:
     var CONFIG = { contactWebhook: 'https://your-n8n-instance...' }
   Replace with your real n8n webhook URL.
   OR change the <form> action to a Formspree / Web3Forms URL.

7. CONNECT ENROLLMENT FORM & STUDENT PORTAL
   In pages/german-language.html (and homepage), find:
     var CONFIG = { webhookURL: '...', flutterwaveKey: '...' }
   Replace with your real n8n and Flutterwave credentials.

8. ADD A MAP
   In pages/contact.html, find the <!-- MAP --> comment block.
   Follow Option A (Google Maps) or Option B (OpenStreetMap).

9. PUBLISH ONLINE
   Upload the entire limburg-website/ folder to any web host.
   Recommended hosts: Hostinger, Namecheap, Netlify (free).
   Point your domain www.limburggermanculturalcenter.cm to it.

================================================================
COLOR REFERENCE (to match brand in external tools)
================================================================

  Primary Red:     #C41E3A
  Hover Red:       #E8324F
  Gold:            #C9A84C
  Deep Black:      #080808
  Warm White:      #F8F6F1
  Off White:       #EEEAE2
  Body Gray:       #6B6660
  Cameroon Green:  #007A5E
  Cameroon Red:    #CE1126
  Cameroon Yellow: #FCD116

================================================================
PAGES SUMMARY
================================================================

  index.html          — Hero, Services grid, Why Choose, German
                        Language enroll form, Membership pricing,
                        Heritage cards, Testimonials, News, Contact,
                        Donate section, Footer

  german-language.html — Intake banner with countdown, Level cards
                        (A1–B2) with skill descriptions, Registration
                        form (Physical/Online), Schedule, Student
                        Portal with Jitsi classroom

  services.html       — All 8 services with full descriptions,
                        image slots, feature lists, pricing, CTAs

  about.html          — Founding story, Mission & Values, History
                        timeline (1884–2026), Team, Partners

  heritage.html       — 7 tour packages, German colonial history,
                        Heritage sites, Book a tour CTA

  news.html           — Featured article, sidebar news, articles
                        grid with category filter, Upcoming events,
                        Newsletter signup

  contact.html        — Contact info blocks, Contact form (n8n),
                        Map placeholder, WhatsApp float button

================================================================
