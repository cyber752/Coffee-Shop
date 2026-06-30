<div align="center">
  <h1>☕ Coffee Shop App</h1>
  <p>A beautiful, interactive single-page application for customizing your perfect coffee order.</p>

  <a href="https://cyber752.github.io/Coffee-Shop/" target="_blank">
    <img src="https://img.shields.io/badge/View_Live_Demo-Click_Here-1db954?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
  </a>
  <br />
  <br />
  
  <img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" alt="JavaScript" />
</div>

---

## ✨ Features

- **Real-Time Visual Updates**: Watch your coffee cup fill and change color dynamically based on your drink selection (Espresso, Latte, Cappuccino, Matcha, Chai).
- **Customizable Sizes & Milk**: Choose between Small, Medium, or Large, and pick your preferred milk (Regular, Oat, Almond, Soy, or None).
- **Interactive Extras**: Add extra shots, vanilla syrup, caramel syrup, or whipped cream, and see animated badges pop up around your cup!
- **Dynamic Pricing**: The order summary automatically calculates the total price of your customized beverage as you interact with the options.

## 🚀 Getting Started

To run this project locally, you don't need any complex build tools or servers. It's built with pure Vanilla web technologies!

1. **Clone the repository** (or download the ZIP):
   ```bash
   git clone https://github.com/cyber752/coffee-shop.git
   ```
2. **Navigate to the folder**:
   ```bash
   cd coffee-shop
   ```
3. **Open the App**: 
   Simply double-click `index.html` to open it in your default web browser, or drag and drop it into a new tab!

## 🧠 Architecture Overview

This project perfectly demonstrates how the core building blocks of the web can harmonize to create a dynamic experience:

- **HTML (`index.html`)**: The structural foundation. It holds the intuitive input panels and the empty coffee cup container.
- **CSS (`styles.css`)**: The visual magic. It utilizes modern layouts (Flexbox/Grid), but more importantly, it uses **CSS custom properties (variables)** and `transitions` to smoothly animate the liquid filling the cup when the state changes.
- **JavaScript (`script.js`)**: The brains of the operation. It attaches event listeners to all inputs, manages a central `order` state object, and directly manipulates the DOM and CSS variables to visually reflect the order and calculate the final receipt.

## 🛠️ How it Works Under the Hood

1. **State Management**: A centralized `order` object keeps track of the current drink, size, milk, and an array of selected extras.
2. **Reactivity**: Every radio button and checkbox change triggers an update to the state object and subsequently calls two main rendering functions: `updateCup()` and `updateSummary()`.
3. **CSS Variable Animations**: Instead of complex JavaScript animation logic, `script.js` simply overrides variables like `--fill-colour` and `--fill-height` on the `.cup` HTML element. The CSS `transition` property handles the smooth visual interpolation automatically!

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/coffee-shop-app/issues).

---
<div align="center">
  <i>Built with ❤️ for coffee lovers everywhere.</i>
</div>
