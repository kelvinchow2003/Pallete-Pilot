# 🎨 Palette Pilot

## Overview
Palette Pilot is a sleek, intuitive web application designed for designers, developers, and creatives who need fast, beautiful color inspiration. It combines two powerful tools in one elegant interface:

- **Random Palette Generator** – Instantly generate stunning 5-color palettes with a single click.
- **Image Color Picker** – Extract dominant or precise colors directly from any image you upload.

Built with a soft, neumorphic UI for a calming, tactile experience — no harsh edges, no glare. Just pure color exploration.

## ✨ Features

### 🌀 Random Palette Generator
- Generates 5 unique, random hex colors on demand.
- Background subtly shifts to match the first color for immersive feedback.
- Click any color block to copy its hex code instantly.
- Visual feedback with smooth hover animations and copy notifications.

### 🖼️ Image Color Picker
- Upload any JPG, PNG, or GIF image.
- Hover over the image to see the exact RGB color under your cursor in real time.
- See the hex code update dynamically as you move.
- One-click copy for the currently hovered color.
- Works with local files and respects CORS where possible.
- Generate a palette thats tailoured to the image you uploaded

### 🧘‍♀️ Soft UI Design
- Neumorphic styling: Gentle shadows, embossed buttons, and subtle depth.
- Smooth animations: All interactions feel tactile and responsive.
- Lightweight & fast: No external frameworks beyond Tailwind CSS.
- Fully responsive: Looks beautiful on mobile, tablet, or desktop.

### 💡 UX Extras
- Copy success notifications (toast-style and modal fallback).
- High-contrast text automatically chosen based on color brightness.
- Canvas-based color sampling for pixel-perfect accuracy.
- Zero dependencies beyond Tailwind and Google Fonts.

## 🚀 How to Use

### Generate a Palette:
Click **“Generate New Palette”** to create a fresh 5-color scheme. Click any color to copy its hex code.

### Pick Colors from Images:
Click the **“Choose File”** button under the Image Picker section, select an image, then hover over it to sample colors. Click **“Copy Hex”** to save the color under your cursor.

Enjoy! Use your palettes for design systems, CSS variables, Figma themes, or just pure visual delight.

## 🛠️ Technical Details
- **Frontend:** Pure HTML, CSS, and JavaScript (no React, Vue, etc.)
- **Styling:** Tailwind CSS + Custom Neumorphic CSS
- **Fonts:** Google Fonts — Inter (clean, modern, highly readable)
- **Color Sampling:** Canvas `getImageData()` for pixel-accurate extraction
- **Clipboard:** Uses `document.execCommand('copy')` for broad compatibility
- **CORS Handling:** Uses `crossOrigin="Anonymous"` for external images (local files always work)
- **Performance:** `willReadFrequently: true` enabled on canvas context for smooth hover

## 📱 Responsive Design
Palette Pilot is fully responsive and optimized for:
- **Mobile:** Vertical layout, touch-friendly buttons
- **Tablet:** Balanced grid with larger color blocks
- **Desktop:** Split-panel layout for side-by-side tool use

## 🔧 How to Run Locally
1. Save the HTML file as `index.html`
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. No server required — works entirely in the browser!
