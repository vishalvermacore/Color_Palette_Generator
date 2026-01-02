# 🎨 Color Palette Generator | HTML, CSS & Vanilla JavaScript

A **Color Palette Generator built with HTML, CSS, and Vanilla JavaScript** that allows users to generate random color palettes and instantly copy HEX color codes to the clipboard.

This project demonstrates **core front-end development concepts** such as DOM manipulation, event delegation, responsive UI design, and usage of the modern Clipboard API — without relying on any JavaScript frameworks or libraries.

Ideal for:
- JavaScript beginners
- Front-end developer portfolios
- UI/UX practice projects
  
---


## 📸 Screenshots

![Palette Generator]()
---

## 🚀 Features

- Random color palette generation
- Five HEX color codes per palette
- One-click copy to clipboard
- Copy by clicking color block or copy icon
- Visual success feedback after copying
- Responsive CSS Grid layout
- Smooth hover and interaction animations
- Built using pure HTML, CSS, and JavaScript

---

## 🛠️ Tech Stack

- **HTML5** – Semantic structure
- **CSS3** – Grid, Flexbox, responsive design, animations
- **JavaScript (ES6)** – DOM manipulation, event handling, logic
- **Font Awesome** – Icons for copy and feedback

No frameworks. No build tools. No dependencies.

---

## 📁 Project Structure
color-palette-generator/
│── index.html # Application structure
│── style.css # Styling and responsive layout
│── script.js # Palette generation & clipboard logic
└── README.md # Project documentation


---

## 📖 How the Color Palette Generator Works

### 🔹 Palette Generation Logic
- Clicking the **Generate Palette** button triggers random HEX color creation.
- Colors are generated using a hexadecimal character set (`0–9`, `A–F`).
- Five colors are generated per click and rendered dynamically.

### 🔹 Clipboard Copy Functionality
- Users can copy a color by:
  - Clicking the copy icon
  - Clicking directly on the color block
- Uses the **Clipboard API** to securely write text to the clipboard.
- A check icon briefly replaces the copy icon to confirm success.

### 🔹 Event Delegation
- A single event listener on the palette container manages all click actions.
- Improves performance and keeps the code clean and scalable.

---

## ✏️ Customization Guide

### Change Number of Colors
Modify the loop in `script.js`:
```js
for (let i = 0; i < 5; i++) {
  colors.push(generateRandomColor());
}

