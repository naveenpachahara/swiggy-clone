# 🍔 Swiggy Clone — Food Delivery Web Application

A modern **Swiggy-inspired food delivery web application** built with **React.js**, designed to provide a smooth and interactive experience for discovering restaurants, browsing menus, searching for food, managing a cart, and completing checkout.

The project focuses on building a real-world food delivery interface using **reusable React components, Redux state management, dynamic routing, and responsive UI patterns**.

---

## 🚀 Live Project

🔗 **GitHub Repository:**
https://github.com/naveenpachahara/swiggy-clone

---

## ✨ Features

### 🏠 Home Page

* Clean Swiggy-inspired landing page
* Food category browsing
* Restaurant discovery
* Multiple food sections
* Dynamic content rendering
* Responsive layout

### 🍽️ Restaurant Discovery

* Browse restaurants
* Restaurant cards with ratings and information
* Restaurant-specific pages
* Menu browsing
* Food item categorization
* Restaurant information section

### 🔎 Food Search

* Search food items
* Search-based food filtering
* Dedicated search interface
* Dynamic rendering of matching food items

### 🍕 Food Menu

* Restaurant-specific menus
* Reusable food cards
* Food item details
* Category-based menu sections
* Add items directly to cart

### 🛒 Shopping Cart

* Add food items to cart
* Remove items from cart
* Centralized cart state
* Dynamic cart updates
* Cart item management
* Checkout flow

### 💳 Checkout

* Dedicated checkout page
* Order summary
* Cart-based pricing
* Simple checkout experience

### 🛍️ Grocery

* Dedicated grocery section
* Grocery categories
* Reusable grocery cards
* Grocery item browsing

### 🍴 Dine

* Dedicated dining section
* Restaurant/dining cards
* Dining options
* Reusable components

### ⚡ Loading Experience

* Shimmer/loading UI
* Better user experience while content is loading

---

## 🛠️ Tech Stack

| Technology            | Usage                     |
| --------------------- | ------------------------- |
| **React.js**          | Frontend UI development   |
| **JavaScript (ES6+)** | Application logic         |
| **Redux**             | Global state management   |
| **Redux Toolkit**     | Cart state management     |
| **React Router**      | Client-side routing       |
| **CSS**               | Styling and responsive UI |
| **Parcel**            | Development & bundling    |
| **Git & GitHub**      | Version control           |

---

## 🧠 Key Technical Concepts

This project was built to practice and demonstrate real-world frontend development concepts.

### ⚛️ Component-Based Architecture

The application is divided into small reusable components instead of keeping everything inside a single component.

Examples:

```text
FoodCard
RestaurantCard
GroceryCard
DineCard
MenuCard
Header
Checkout
SearchFood
```

This makes the application easier to maintain, debug and extend.

---

### 🔄 Redux State Management

The shopping cart is managed using Redux.

```text
User
  ↓
Add Food
  ↓
Redux Store
  ↓
Cart Slice
  ↓
Cart UI
  ↓
Checkout
```

Using centralized state management prevents different components from maintaining separate versions of the cart.

---

### 🧭 Client-Side Routing

Different sections of the application are handled through routes instead of traditional page reloads.

```text
Home
 ├── Restaurant
 │    └── Restaurant Menu
 │
 ├── Search
 │
 ├── Grocery
 │
 ├── Dine
 │
 ├── Cart
 │
 └── Checkout
```

---

## 📂 Project Structure

```text
swiggy-clone/
│
├── App.js
├── Header.js
├── Home.js
├── SecondaryHome.js
│
├── Restaurant.js
├── RestaurantMenu.js
├── RestCard.js
├── RestHeader.js
├── RestInfo.js
│
├── MenuCard.js
│
├── FoodCard.js
├── FoodData.js
├── FoodOption.js
│
├── Grocery.js
├── GroceryCard.js
├── GroceryOption.js
│
├── DineCard.js
├── DineData.js
├── DineOption.js
│
├── SearchFood.js
│
├── CartSlicer.js
├── Checkout.js
├── stores.js
│
├── Shimmer.js
│
├── index.css
├── index.html
├── package.json
└── package-lock.json
```

---

## 🔥 Application Flow

```text
                    ┌───────────────┐
                    │   Home Page   │
                    └───────┬───────┘
                            │
            ┌───────────────┼────────────────┐
            ↓               ↓                ↓
      Restaurants        Search           Grocery
            │               │                │
            ↓               ↓                ↓
      Restaurant        Food Results     Grocery Items
         Menu                │
            │                │
            └────────┬───────┘
                     ↓
                Add To Cart
                     │
                     ↓
              ┌─────────────┐
              │ Redux Store │
              └──────┬──────┘
                     ↓
                   Cart
                     │
                     ↓
                 Checkout
```

---

## 🧩 Reusable Components

One of the main goals of this project was to avoid duplicating UI logic.

For example, food items are rendered using reusable components:

```text
FoodCard
   ↓
Food Data
   ↓
Reusable Food UI
```

Similarly:

```text
Restaurant Data
      ↓
   RestCard
      ↓
Restaurant Listing
```

and:

```text
Grocery Data
      ↓
 GroceryCard
      ↓
Grocery Listing
```

This component-driven approach makes it easier to add new features without rewriting existing UI.

---

## 🛒 Cart Architecture

The cart uses Redux for centralized state management.

```text
Component
    ↓
Dispatch Action
    ↓
Cart Slice
    ↓
Redux Store
    ↓
Updated Cart State
    ↓
Cart Component
```

This allows the cart state to remain consistent across different parts of the application.

---

## 🔍 Search Architecture

The search functionality provides a dedicated interface for finding food items.

```text
Search Input
     ↓
User Query
     ↓
Food Data
     ↓
Filter / Match
     ↓
Matching Food Cards
```

This creates a simple and intuitive food discovery experience.

---

## 📱 Responsive UI

The interface is designed with responsive layouts so that the application can adapt to different screen sizes.

The styling focuses on:

* Flexible layouts
* Responsive cards
* Mobile-friendly navigation
* Consistent spacing
* Reusable UI patterns

---

## ⚡ Performance & UX

The application uses a few techniques to provide a smoother user experience:

* Component-based rendering
* Reusable UI components
* Redux for predictable state updates
* Shimmer loading UI
* Client-side navigation
* Structured data modules

---

## 🧪 Main Functional Areas

| Module         | Functionality               |
| -------------- | --------------------------- |
| 🏠 Home        | Food & restaurant discovery |
| 🍽️ Restaurant | Restaurant browsing         |
| 📋 Menu        | Restaurant menu             |
| 🔎 Search      | Search food items           |
| 🛒 Cart        | Manage selected items       |
| 💳 Checkout    | Order summary & checkout    |
| 🛍️ Grocery    | Grocery browsing            |
| 🍴 Dine        | Dining discovery            |

---

## 🏗️ What I Learned

Building this project helped me strengthen my understanding of:

* React component architecture
* Props and state
* React Hooks
* Redux & Redux Toolkit
* Global state management
* React Router
* Dynamic rendering
* Reusable components
* Search/filter functionality
* Cart management
* Responsive CSS
* Project structuring
* Git & GitHub workflow

---

## 🔮 Future Improvements

The project can be extended with:

* 🔐 User authentication
* 👤 User profiles
* 📍 Location-based restaurant discovery
* 💳 Real payment integration
* 📦 Order tracking
* ❤️ Wishlist functionality
* ⭐ Restaurant reviews & ratings
* 🔔 Order notifications
* 🗄️ Backend integration
* 🛢️ Database integration
* 📱 Progressive Web App support

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/naveenpachahara/swiggy-clone.git
```

### 2. Navigate to the project

```bash
cd swiggy-clone
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm start
```

Then open the local URL shown in your terminal.

---

## 📌 Project Highlights

> A frontend-focused food delivery application demonstrating practical usage of **React.js, Redux, routing, reusable components, dynamic rendering, search, cart management, and checkout flow**.

### ⭐ Key Highlights

* ⚛️ React-based architecture
* 🔄 Redux-powered cart
* 🧩 Highly reusable components
* 🧭 Client-side routing
* 🔎 Food search
* 🍽️ Restaurant & menu browsing
* 🛒 Cart management
* 💳 Checkout flow
* 🛍️ Grocery section
* 🍴 Dine section
* ⚡ Shimmer loading UI
* 📱 Responsive design

---

## 👨‍💻 Author

### Naveen Pachahara

**B.Tech Computer Science Engineering**

Interested in:

* Full Stack Development
* MERN Stack
* Frontend Development
* Software Engineering
* Data Structures & Algorithms

### 🔗 Connect With Me

**GitHub:**
https://github.com/naveenpachahara

**Project:**
https://github.com/naveenpachahara/swiggy-clone

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

---

### 📄 License

This project was created for **educational and portfolio purposes**.
