
# 🛍 React + Firebase E-Commerce

A basic e-commerce application built with **React** for the frontend and **Firebase** for authentication and database.  
It supports user signup/login, product browsing, cart management, and a simulated checkout process with order tracking.

---

## 🚀 Features

- **User Authentication** with Firebase (Email/Password)
- **Protected Routes** so only logged-in users can browse and shop
- **Firestore Integration** for fetching products
- **Cart System** with `localStorage` persistence
- **Checkout Flow** that stores orders in the app's state
- **Responsive UI** built with React components

---

## 🛠 Tech Stack

- **Frontend:** React, React Router
- **Backend:** Firebase Firestore, Firebase Authentication
- **State Management:** React Hooks (`useState`, `useEffect`)
- **Storage:** LocalStorage (cart persistence)

---

## 📦 Setup & Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
   cd YOUR_REPO
    ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Setup Firebase**

   * Go to [Firebase Console](https://console.firebase.google.com/) and create a project.
   * Enable **Authentication → Email/Password**.
   * Create a **Firestore Database** in *Test Mode*.
   * Add a `products` collection in Firestore.
     Each product document should look like:

     ```json
     {
       "sku": "SKU123",
       "name": "Red Dress",
       "price": 49.99,
       "image": "https://i.ibb.co/example/red-dress.jpg",
       "description": "Stylish red dress perfect for parties."
     }
     ```
   * Copy your Firebase config from the console and place it in `src/firebase/firebase.js`.

4. **Run the development server**

   ```bash
   npm start
   ```

---

## 📌 Future Improvements

* Store orders in Firestore instead of local state
* Add a payment gateway (Stripe, PayPal)
* Create an admin dashboard for managing products

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

