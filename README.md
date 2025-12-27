# Shopify Snippets Library

Reusable **Shopify Liquid snippets** for common store customizations. All examples use **placeholders** so you can adapt them safely without exposing client-specific data.

---

## 📂 Snippets Included

### 1. WhatsApp Button (`snippets/WhatsApp-Button.liquid`)
Add a floating WhatsApp contact button to your store.

**Features:**
- Round button with WhatsApp icon.
- Customizable phone number and message.
- Responsive floating button.
- Easy to style with CSS.

**Usage:**  
```liquid
{% render 'WhatsApp-Button' %}
```

### 2. Events List – Horizontal Stripes (`snippets/events-list.liquid`)
Display a list of upcoming events in a horizontal stripe layout.

**Features:**

- Locale detection (BR vs others)
- Each row displays date and title in PT/EN
- Responsive design with styled date pill and event title

**Usage:** 
```liquid
{% render 'events-list' %}
```

### 3. Free Shipping Bar (`snippets/free-shipping-bar.liquid`)

Show a progress bar encouraging customers to reach the free shipping threshold.

**Features:**

- Dynamic calculation based on cart total
- Customizable threshold and messages
- Animated progress bar
- Responsive design

**Usage:** 
```liquid
{% render 'free-shipping-bar' %}
```

### 4. Live Event Embed (`snippets/live-event.liquid`)

Embed a live event (e.g. Vimeo stream) with multilingual support and a newsletter reminder form.

**Features:**

- Locale detection (BR vs others)
- Event title, description, date, and details using placeholders
- Newsletter form integration
- Responsive design

**Usage:** 
```liquid
{% render 'live-event' %}
```

### 5. Product Upsell Card (`snippets/product-upsell-card.liquid`)

Suggest related products to increase average order value.

**Features:**

- Pulls product data dynamically via handle
- Displays product image, title, and price
- Styled card with shadow and rounded corners
- Call-to-action button with cart icon

**Usage:** 
```liquid
{% render 'product-upsell-card' %}
```

### 6. Promo Countdown Timer (`snippets/promo-countdown-timer.liquid`)

Create urgency with a countdown timer for promotions.

**Features:**

- Configurable end date
- Real-time countdown (days, hours, minutes, seconds)
- Modern design with gradient background
- Easy to reuse for multiple campaigns

**Usage:**
```liquid
{% render 'promo-countdown-timer' %}
```

🛠 Notes

All dates, titles, and links are placeholders. Replace them with your actual project data.
Snippets are designed to be generic and reusable.
You can mix and match snippets to build custom Shopify themes.

📜 License

This repository is licensed under the MIT License. You are free to use, modify, and distribute these snippets in your own projects.

