# Shopify Liquid Snippets

This repository contains reusable **Shopify Liquid snippets** for embedding live events and listing upcoming events. All examples use **placeholders** so you can adapt them safely without exposing client-specific data.

---

## 📂 Snippets Included

### 1. Live Event Embed (`snippets/live-event.liquid`)
A reusable block for embedding a live event (e.g., Vimeo stream) with multilingual support (Portuguese and English) and a newsletter reminder form.

**Features:**
- Detects user locale (`BR` or `pt`) and switches UI text accordingly.
- Displays event title, description, date, and details with placeholders.
- Embeds a video iframe (replace with your own Vimeo or other provider link).
- Includes a newsletter form using Shopify's `customer` form.
- Responsive design for desktop and mobile.

**Usage:**
1. Copy the snippet into your Shopify theme under `/snippets/live-event.liquid`.
2. Replace placeholder variables:
   - `EVENT_TITLE_PT` / `EVENT_TITLE_EN`
   - `EVENT_DESCRIPTION_PT` / `EVENT_DESCRIPTION_EN`
   - `EVENT_DATE_PT` / `EVENT_DATE_EN`
   - `EVENT_DETAILS_PT` / `EVENT_DETAILS_EN`
   - `INFO_TEXT_PT` / `INFO_TEXT_EN`
   - `https://example.com/live` → your event page
   - `INSTAGRAM_LOGO_URL` and `BRAND_LOGO_URL` → your brand assets
3. Insert the snippet in a template:
   ```liquid
   {% render 'live-event' %}
4. Adjust CSS styles as needed for your brand identity.

2. Events List (Horizontal Stripes) (snippets/events-list.liquid)
Displays a list of upcoming events in a horizontal stripe layout. Supports multilingual content (Portuguese for Brazil, English for other locales).

Features
- Locale detection (BR vs others).
- Each event line contains:
- Date in Portuguese
- Date in English
- Title in Portuguese
- Title in English
- Responsive design with styled date pill and event title.

Usage
- Copy the snippet into your Shopify theme under /snippets/events-list.liquid.
- Edit the {% capture lives %} block:
DatePT||DateEN||TitlePT||TitleEN
- Example:
01/01/2026 — 20:15 BRT||Jan 01, 2026 — 8:15 PM BRT||EVENT_TITLE_PT||EVENT_TITLE_EN
- Insert the snippet in a template:
{% render 'events-list' %}
- Customize CSS styles to match your brand identity.

🛠 Notes
- All dates, titles, and links in this repository are placeholders. Replace them with your actual project data.
- The snippets automatically switch between Portuguese and English depending on the user's locale.
- Designed to be generic and reusable, so you can adapt them for multiple projects.

📜 License
This repository is licensed under the MIT License. You are free to use, modify, and distribute these snippets in your own projects.
