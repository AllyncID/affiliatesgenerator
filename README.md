# Affiliates MineHive Generator

A simple web-based promo poster generator that lets users enter a promo code, preview the result in real time, and download a 1080x1080 PNG poster.

## Overview

**affiliatesgenerator** is a lightweight static HTML tool designed to generate promotional poster images for affiliate or discount campaigns. Users can type a promo code, instantly preview it on the poster layout, and export the final result as a PNG image.

The project uses a custom poster canvas, scales the preview responsively, and captures the final design using **html2canvas**.

## Features

- Real-time promo code preview
- 1080x1080 poster output
- One-click PNG download
- Responsive preview scaling
- Tailwind CSS based UI
- SweetAlert2 notifications
- Custom promo font support (`IntegralCF`)
- External background image support

## Tech Stack

- HTML
- Tailwind CSS (CDN)
- JavaScript
- html2canvas
- SweetAlert2
- Font Awesome

## How It Works

1. Enter a promo code in the input field.
2. The poster preview updates automatically.
3. Click **Download Hasil** to export the poster.
4. The result is saved as a PNG file.

## Setup

Since this project is a static web app, no build process is required.

### Option 1: Open directly

Just open `index.html` in your browser.

### Option 2: Host on a static server

You can also deploy it on any static hosting service such as:

- GitHub Pages
- Netlify
- Vercel
- Any shared hosting

## Customization

### Change the default promo code

Edit the input value inside `index.html`:

```html
<input id="codeField" value="ALLYNC10">
```

### Change the background image

Update the background image URL in the script section:

```js
const backgroundImageURL = 'https://i.imgur.com/nObbmIX.png';
```

Make sure the image URL is **public** and supports **CORS**, otherwise `html2canvas` may fail during export.

### Change the promo font

The project uses a custom font loaded from:

```text
font/integral.otf
```

Replace it with your own font if needed.

## Project Structure

```text
.
├── font/
├── images/
└── index.html
```

## Notes

- Poster resolution is fixed at **1080x1080**.
- Promo text is automatically transformed to uppercase.
- If the input is empty, the preview falls back to `KODE`.
- Export depends on browser support and external image accessibility.

## Use Cases

This project is suitable for:

- Affiliate promo poster generation
- Discount code campaigns
- Social media promotional assets
- Simple internal marketing tools

## Future Improvements

Potential enhancements:

- Background image upload from local device
- Multiple templates
- Color and text position customization
- Batch poster generation
- Automatic branding presets

---

Built as a lightweight promo poster generator for affiliate and discount campaigns.
