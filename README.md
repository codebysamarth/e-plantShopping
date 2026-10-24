# Paradise Nursery Shopping Application

A responsive e-commerce web application for an online plant shop called **Paradise Nursery**, developed as the final project submission for the Coursera course **Developing Front-End Apps with React** (IBM).

---

## Project Overview

Paradise Nursery is an intuitive single-page shopping application that allows users to browse a wide variety of indoor houseplants, view details including plant images, names, descriptions, and prices, add plants to a shopping cart, and manage their cart dynamically. 

The application utilizes **React** for building the component-based user interface and **Redux Toolkit** for robust global state management of the shopping cart.

---

## Key Features

- **Landing Page (`App.jsx`, `App.css`)**:
  - Welcoming hero section with high-quality background greenhouse imagery.
  - Company branding: *"Paradise Nursery - Where Green Meets Serenity"*.
  - Informative **About Us** section describing company background, mission, and dedication to plants.
  - Interactive **Get Started** button transitioning smoothly to the product catalog.

- **Product Listing Catalog (`ProductList.jsx`)**:
  - Organized into distinct houseplant categories:
    - *Air Purifying Plants*
    - *Aromatic Fragrant Plants*
    - *Insect Repellent Plants*
    - *Medicinal Plants*
    - *Low Maintenance Plants*
  - Displays 6 unique houseplants per category with thumbnail images, names, descriptions, and prices.
  - Dynamic **Add to Cart** buttons:
    - Adds the selected plant to the Redux store.
    - Disables automatically and changes text to *"Added to Cart"* once added.
    - Updates the navbar shopping cart count in real time.

- **Navigation Bar (`ProductList.jsx`)**:
  - Present consistently across both Product Listing and Cart views.
  - Includes links to **Home** (returns to landing page), **Plants** (browses plant catalog), and **Cart** (views shopping cart).
  - Dynamic shopping cart badge displaying the total item count.

- **Shopping Cart Management (`CartItem.jsx`, `CartSlice.jsx`)**:
  - Global cart state managed with **Redux Toolkit** (`addItem`, `removeItem`, `updateQuantity`).
  - View all added plants with thumbnail, plant name, and unit cost.
  - Increment (`+`) and Decrement (`-`) buttons to adjust plant quantities dynamically.
  - Auto-removal or single-click **Delete** button to remove items from the cart.
  - Real-time calculation of subtotal per plant item and grand total amount for the entire cart.
  - **Continue Shopping** button returning to the product listing.
  - **Checkout** button providing instant user feedback (*"Coming Soon"*).

---

## Technologies Used

- **React 18** - Component-based frontend architecture
- **Redux Toolkit & React-Redux** - Centralized state management for shopping cart
- **Vite** - Fast next-generation frontend build tooling
- **CSS3** - Responsive styling, Flexbox layout, and CSS animations
- **HTML5 & SVG** - Semantic markup and vector icons

---

## Installation & Setup Instructions

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd e-plantShopping
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## Course Submission Details

- **Course:** Developing Front-End Apps with React
- **Assignment:** Final Project: Paradise Nursery Shopping Application
- **Author:** Samarath
