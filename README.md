# 🛒 E-Commerce Platform

A modern, responsive, and scalable **e-commerce frontend** inspired by platforms like Amazon and Flipkart. The project provides a complete shopping experience with product API integration, cart management, GST calculation, coupon codes, delivery charges, checkout, order tracking, seller dashboard, and admin panel.

## 🚀 Features

### 👤 Customer

* 🏠 Modern e-commerce homepage
* 🔍 Product search and suggestions
* 🗂️ Categories and subcategories
* 🛍️ Product listing and filtering
* ↕️ Product sorting
* 📦 Product details
* ❤️ Wishlist
* 🛒 Shopping cart
* 🔢 Product quantity management
* 🎟️ Coupon codes
* 🧾 GST calculation
* 🚚 Delivery charge calculation
* 💳 Checkout and payment UI
* 📍 Address management
* 📦 Order management
* 🚛 Order tracking
* 🔄 Return and refund UI
* ⭐ Product ratings and reviews
* 🔔 Notifications
* 👤 User profile
* 🧾 Order invoice

### 💰 Pricing System

The application includes a centralized pricing system supporting:

* Product price
* Product discounts
* GST
* Coupon discounts
* Delivery charges
* Final payable amount

### 🚚 Delivery

Default delivery rule:

* Orders below ₹2,000 → ₹99 delivery charge
* Orders ₹2,000 or above → Free delivery

These values can be configured according to business requirements.

### 🎟️ Coupon System

Supports:

* Percentage discount
* Fixed amount discount
* Minimum order value
* Maximum discount
* Expiry date
* Product-specific coupons
* Category-specific coupons
* First-order coupons

### 📦 Product API

Products are loaded through an API instead of being directly hardcoded into components.

The architecture supports:

* Product listing
* Product details
* Search
* Categories
* Filtering
* Sorting
* Pagination
* Related products
* Product recommendations

A mock API/service layer can be used during frontend development and replaced with a real backend later.

---

## 🏪 Seller Dashboard

The project also includes a seller interface for managing an online store.

### Features

* Seller dashboard
* Add products
* Edit products
* Delete products
* Inventory management
* Order management
* Sales analytics
* Product performance
* Customer information
* Reviews
* Coupon management

---

## 👨‍💼 Admin Dashboard

The admin panel provides complete platform management.

### Features

* Dashboard
* User management
* Seller management
* Product management
* Category management
* Order management
* Coupon management
* Review management
* Sales reports
* Revenue analytics
* Platform statistics

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* JavaScript
* Tailwind CSS

### State Management

* Redux Toolkit

### API & Forms

* Axios
* React Hook Form

### UI & Visualization

* Lucide React
* Framer Motion
* Recharts
* Sonner / React Toastify

### Development

* Git
* GitHub
* ESLint

---

## 📁 Project Structure

```text
src/
│
├── assets/
│
├── components/
│   ├── common/
│   ├── navbar/
│   ├── footer/
│   ├── product/
│   ├── cart/
│   ├── checkout/
│   ├── seller/
│   └── admin/
│
├── pages/
│   ├── Home/
│   ├── Products/
│   ├── ProductDetails/
│   ├── Search/
│   ├── Cart/
│   ├── Checkout/
│   ├── Orders/
│   ├── Wishlist/
│   ├── Profile/
│   ├── Auth/
│   ├── Seller/
│   └── Admin/
│
├── layouts/
│   ├── UserLayout.jsx
│   ├── SellerLayout.jsx
│   └── AdminLayout.jsx
│
├── redux/
│   ├── store.js
│   └── slices/
│       ├── authSlice.js
│       ├── productSlice.js
│       ├── cartSlice.js
│       ├── wishlistSlice.js
│       ├── couponSlice.js
│       └── orderSlice.js
│
├── services/
│   ├── api.js
│   ├── productApi.js
│   ├── couponApi.js
│   └── orderApi.js
│
├── utils/
│   ├── priceCalculator.js
│   ├── gstCalculator.js
│   ├── couponCalculator.js
│   └── deliveryCalculator.js
│
├── hooks/
├── routes/
├── App.jsx
└── main.jsx
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd ecommerce-frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file:

```env
VITE_API_BASE_URL=your_api_url
```

### 4. Start development server

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:5173
```

---

## 🔌 API Architecture

The frontend uses a centralized API architecture:

```text
React Components
       ↓
Redux Toolkit
       ↓
API Services
       ↓
Axios
       ↓
Backend / Product API
```

This makes it easy to replace the mock API with a real backend such as:

* Django REST Framework
* FastAPI
* Node.js / Express

---

## 💵 Price Calculation Flow

```text
Product Price
      ↓
Quantity
      ↓
Product Discount
      ↓
Subtotal
      ↓
Coupon Discount
      ↓
GST
      ↓
Delivery Charge
      ↓
Final Payable Amount
```

The pricing logic is centralized to avoid inconsistent calculations between the cart, checkout, and order pages.

> **Note:** GST, discounts, delivery charges, and final payable amounts should be validated by the backend in a production environment. Frontend calculations are primarily for display and user experience.

---

## 📱 Responsive Design

The application is designed for:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📲 Tablet

The UI uses responsive layouts and reusable components instead of separate mobile and desktop applications.

---

## 🔮 Future Improvements

* Real payment gateway integration
* Real-time order tracking
* AI-based product recommendations
* Advanced product search
* Elasticsearch integration
* Email notifications
* SMS/OTP verification
* Multiple seller support
* Product comparison
* PWA support
* Performance optimization
* Backend integration
* Cloud deployment

---

## 📌 Project Status

🚧 **Currently under development**

The project is being developed in phases, starting with the customer shopping experience and gradually adding seller and admin functionality.

---

## 👨‍💻 Author

**Omm Abinash Barik**

B.Tech CSE (AI & ML)

Interested in:

* Software Development
* Artificial Intelligence
* Machine Learning
* Full-Stack Development

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and Oxlint's TypeScript related rules in your project.
