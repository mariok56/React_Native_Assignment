# 📱 E-Commerce Social App – React Native Mobile Application

**E-Commerce Social App** is a full-featured mobile application built with **React Native** and **TypeScript**.  
It combines a **social feed** with an **e-commerce product catalogue**, allowing users to browse products, add new ones, view product details, and interact with simple social posts.

The project demonstrates:
- Modern React Native architecture
- TypeScript best practices
- Atomic design methodology
- Form validation with Zod
- Smooth navigation using React Navigation
- Responsive UI and reusable components

---

## ✨ Features

### 🔐 Authentication
- Login & Register forms  
- Input validation using **Zod**  
- Persistent login state  
- Error handling + visual feedback  

---

### 🛒 Products Module
- Product list screen  
- Product details screen  
- Add product screen (with validation)  
- Supports form input, image placeholders, pricing fields, etc.  
- Uses local JSON or mock API for data  

---

### 📨 Social Feed Module
- Simple feed displaying static posts  
- Demonstrates component reuse and list rendering  
- Clean card-based UI  

---

### 🎨 Atomic Design System
Organized into:

- **Atoms** → Button, Input, Text, Card  
- **Molecules** → ProductCard, FormGroup  
- **Organisms** → ProductList, AuthForm  
- **Screens** → Login, Register, Products, ProductDetails, Feed  

Ensures scalable, maintainable UI.

---

### 🧭 Navigation
Using **React Navigation v6**

- **Stack Navigation** → Auth flow + app flow  
- **Tab Navigation** → Feed, Products, Profile  
- Protected screen routing based on login state  

---

### 🎛 State Management
- Lightweight global state using **Context API**  
- Hooks for auth, forms, and data operations  

---

## 📸 Screenshots

> Add your real screenshots inside:  
> `./assets/screenshots/`

### 🔐 Login  
![Login](./assets/screenshots/login.png)

### 📝 Register  
![Register](./assets/screenshots/register.png)

### 🛍️ Product List  
![Products](./assets/screenshots/products.png)

### 📦 Product Details  
![Details](./assets/screenshots/product-details.png)

### ➕ Add Product  
![Add](./assets/screenshots/add-product.png)

### 📨 Feed  
![Feed](./assets/screenshots/feed.png)

---

## 🧰 Tech Stack

### Core
- **React Native**
- **TypeScript**

### UI
- React Native StyleSheet  
- Atomic Design Components  
- Custom theme variables  
- Icons

### Navigation
- **React Navigation** (Stack + Tabs)

### Forms & Validation
- **react-hook-form**
- **zod**

### Data
- Static JSON  
- Local mock services  
- AsyncStorage (state persistence)

### Utilities
- Helper functions  
- Validation schemas  
- Custom hooks  

---

## 📂 Project Structure

```
E-Commerce-Social-App/
├── src/
│   ├── assets/            # Images & icons
│   ├── components/        # Atomic components (atoms, molecules, organisms)
│   ├── data/              # Product JSON data
│   ├── hooks/             # Custom hooks
│   ├── navigation/        # App & Auth navigation stacks
│   ├── screens/           # Application screens
│   ├── context/           # Auth & app context
│   ├── utils/             # Helpers, validation schemas
│   └── App.tsx            # Entry point of the application
├── package.json
└── README.md
```

---

## 🚀 Getting Started

### 1. Install Dependencies
```
npm install
```

### 2. Start Metro Bundler
```
npm start
```

### 3. Run on Android
```
npm run android
```

### 4. Run on iOS (Mac only)
```
npm run ios
```

---

## 🧑‍💻 Scripts

| Command | Description |
|---------|-------------|
| **npm start** | Start Metro bundler |
| **npm run android** | Run on Android device/emulator |
| **npm run ios** | Run on iOS simulator |
| **npm run lint** | Run ESLint |

---

## 🧪 Form Validation (Zod Example)

```ts
const productSchema = z.object({
  title: z.string().min(5),
  price: z.number().min(1),
  description: z.string().min(10),
});
```

---

## 📄 License
This project is for educational and assignment purposes only.

---

## 👤 Author
**Mario Karam**  
GitHub: https://github.com/mariok56  
LinkedIn: https://www.linkedin.com/in/mario-karam-057987341
