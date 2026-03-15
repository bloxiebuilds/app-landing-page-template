# 📖 app-landing-page-template — Instructions

Get your app landing page live in minutes. No coding experience needed.

---

## 📋 Table of Contents

1. [Getting Started](#1-getting-started)
2. [Editing the Config Block](#2-editing-the-config-block)
3. [Customizing Features](#3-customizing-features)
4. [Customizing Pricing](#4-customizing-pricing)
5. [Adding Your Screenshot](#5-adding-your-screenshot)
6. [Setting Your Theme](#6-setting-your-theme)
7. [Deploying to GitHub Pages](#7-deploying-to-github-pages)
8. [FAQ](#8-faq)

---

## 1. Getting Started

1. Go to [github.com/bloxiebuilds/app-landing-page-template](https://github.com/bloxiebuilds/app-landing-page-template)
2. Click **"Use this template"**
3. Name your repo and click **"Create repository"**
4. Open `index.html` in your browser to preview instantly!

---

## 2. Editing the Config Block

Open `index.html` and find the `CONFIG` block near the top. Edit these fields:

| Field | What to put |
|-------|-------------|
| `appName` | Your app or product name |
| `tagline` | One punchy line that sells it |
| `description` | 2-3 sentences about what it does |
| `ctaLabel` | Primary button text e.g. "Get Early Access" |
| `ctaUrl` | Primary button link |
| `ctaSecLabel` | Secondary button text e.g. "See How It Works" |
| `ctaSecUrl` | Secondary button link |
| `accentColor` | Any hex color e.g. `"#a78bfa"` |

---

## 3. Customizing Features

In the `features` array, each item looks like:

```js
{ icon: "⚡", title: "Blazing Fast", desc: "Built for speed from the ground up." },
```

- Change the emoji, title, and description
- Add more by copying a line
- Remove any by deleting its `{ ... },` block

---

## 4. Customizing Pricing

In the `pricing` array, each plan looks like:

```js
{ plan: "Pro", price: "$12", period: "/mo", features: ["Unlimited projects", "Priority support"], cta: "Get started", featured: true },
```

- Set `featured: true` on whichever plan you want highlighted
- Add or remove items in the `features` array
- Change `price` and `period` to match your pricing

---

## 5. Adding Your Screenshot

Find this block in the HTML:

```html
<div class="screen-body">
  <div class="screen-placeholder">
    <strong>Your app screenshot goes here</strong>
    Replace this block with an img tag...
  </div>
</div>
```

Replace the entire inner `<div class="screen-placeholder">` with:

```html
<img src="screenshot.png" alt="App screenshot" style="width:100%;display:block;"/>
```

Put your screenshot file in the same folder as `index.html`.

---

## 6. Setting Your Theme

| Value | Result |
|-------|--------|
| `true` | Always dark |
| `false` | Always light |
| `"toggle"` | Visitor can switch |

---

## 7. Deploying to GitHub Pages

1. Push your repo to GitHub (public)
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Click **Save** — live at:

```
https://YOUR-USERNAME.github.io/app-landing-page-template
```

---

## 8. FAQ

**Q: Can I remove the pricing section?**
Yes — find the `<!-- PRICING -->` comment in the HTML and delete that whole block.

**Q: Can I add more than 6 features?**
Absolutely — just add more objects to the `features` array in the config.

**Q: Can I use this for a SaaS, game, or physical product?**
Yes! It works for anything you want to promote.

---

<p align="center">app-landing-page-template was made by <a href="https://github.com/bloxiebuilds">bloxiebuilds</a></p>
