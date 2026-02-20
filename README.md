# jQuery Shopping Cart

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=flat-square&logo=jquery&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=flat-square&logo=bootstrap&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)

> **Note:** This repository is a fork of [gabrieleromanato/jQuery-sessionStorage-shopping-cart](https://github.com/gabrieleromanato/jQuery-sessionStorage-shopping-cart).

A fully functional client-side shopping cart built with jQuery and the sessionStorage API, featuring PayPal Sandbox integration for checkout.

## Overview

This project implements a complete e-commerce shopping cart workflow using only client-side technologies. Product data, cart state, and order totals are managed entirely through the browser's sessionStorage, making it a lightweight proof-of-concept that requires no server-side backend. The demo is themed as a "Winery" store selling wines, and includes product listing, cart management (add, update quantity, empty), a checkout page with user details validation, and a PayPal Sandbox payment form.

## Features

- **Add to cart** with configurable quantities from the product listing page
- **Cart management** -- update quantities, empty the cart, or continue shopping
- **Shipping rate calculation** based on subtotal thresholds
- **Checkout form** with client-side validation for name, email, and address fields
- **PayPal Sandbox integration** for processing payments
- **sessionStorage persistence** -- cart data survives page navigation within a session
- **Responsive layout** using Bootstrap 4

## Prerequisites

- A modern web browser with JavaScript enabled
- A local web server (optional, for serving files locally) or any static hosting service

## Getting Started

### Installation

```bash
git clone https://github.com/danielcregg/shoppingcart.git
cd shoppingcart
```

### Usage

Open `index.html` directly in your browser, or serve the project directory with any static file server:

```bash
# Using Python
python3 -m http.server 8080

# Using Node.js (npx)
npx serve .
```

Then navigate to `http://localhost:8080` to browse products, add items to your cart, and proceed through checkout.

**Live Demos:**
- [https://danielcregg.github.io/shoppingcart/](https://danielcregg.github.io/shoppingcart/)

**Note:** To enable real PayPal payments, update the following values in `js/jquery.shop.js`:
- `paypalBusinessEmail` -- your PayPal business email
- `paypalURL` -- switch from sandbox to the live PayPal URL
- Shipping rate logic as needed

## Tech Stack

- **Languages:** HTML5, CSS3, JavaScript
- **Library:** jQuery 2.x
- **Framework:** Bootstrap 4
- **Storage:** Browser sessionStorage API
- **Payments:** PayPal Sandbox

## License

This project is licensed under the [MIT License](LICENSE).
