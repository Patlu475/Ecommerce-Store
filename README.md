# E-commerce Clothing Store 👕🛍️

A full-stack e-commerce clothing store built with React.js, Node.js, Express.js, and MongoDB. This application provides a complete online shopping experience with separate interfaces for customers and administrators.

## 📋 Table of Contents

- [Team Members](#team-members)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## 👥 Team Members

- **Nikhal Rajpal** - 023-21-0120
- **Amrat Kukreja** - 023-21-0107  
- **Raveena Roopeja** - 023-21-0155

## ✨ Features

### Customer Features
- 🏪 Browse products by categories (Men, Women, Kids)
- 🛒 Add/Remove items from shopping cart
- 👤 User registration and authentication
- 🔐 Secure login/logout functionality
- 📱 Responsive design for all devices
- 🔍 Product search and filtering

### Admin Features
- 📊 Admin dashboard
- ➕ Add new products
- ✏️ Edit existing products
- 🗑️ Remove products
- 📸 Image upload for products
- 👥 User management

## 🛠️ Tech Stack

### Frontend
- **React.js** (v18.2.0) - UI Library
- **React Router DOM** (v6.21.1) - Client-side routing
- **CSS3** - Styling
- **React Scripts** - Build tool

### Backend
- **Node.js** - Runtime environment
- **Express.js** (v4.18.2) - Web framework
- **MongoDB** - Database
- **Mongoose** (v8.0.4) - ODM for MongoDB
- **JWT** (v9.0.2) - Authentication
- **Multer** (v1.4.5) - File upload handling
- **CORS** (v2.8.5) - Cross-origin resource sharing

### Admin Panel
- **React.js** (v18.2.0) - UI Library
- **Vite** (v5.0.8) - Build tool and dev server
- **React Router DOM** (v6.21.2) - Client-side routing
- **ESLint** - Code linting

## 📁 Project Structure

```
Ecommerce/
├── frontend/                 # Customer-facing React application
│   ├── src/
│   │   ├── Components/       # Reusable React components
│   │   ├── Pages/           # Page components
│   │   ├── Context/         # React context for state management
│   │   ├── App.js           # Main App component
│   │   └── index.js         # Entry point
│   ├── public/              # Static assets
│   └── package.json         # Frontend dependencies
│
├── backend/                  # Node.js/Express.js API server
│   ├── upload/              # Uploaded product images
│   ├── index.js             # Main server file
│   └── package.json         # Backend dependencies
│
├── admin/                    # Admin panel React application
│   ├── src/
│   │   ├── Components/      # Admin UI components
│   │   ├── Pages/          # Admin page components
│   │   ├── assets/         # Static assets
│   │   ├── App.jsx         # Main Admin App component
│   │   └── main.jsx        # Entry point
│   ├── public/             # Static assets
│   └── package.json        # Admin dependencies
│
└── README.md               # Project documentation
```

## 🚀 Installation

### Prerequisites
- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (local installation or MongoDB Atlas)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/AmratKukreja/Ecommerce.git
   cd Ecommerce
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd frontend
   npm install
   ```

3. **Install Backend Dependencies**
   ```bash
   cd ../backend
   npm install
   ```

4. **Install Admin Panel Dependencies**
   ```bash
   cd ../admin
   npm install
   ```

5. **Database Setup**
   - Ensure MongoDB is running on your system
   - Update the MongoDB connection string in `backend/index.js` if needed

## 🏃‍♂️ Usage

### Development Mode

1. **Start the Backend Server**
   ```bash
   cd backend
   node index.js
   ```
   The server will run on `http://localhost:4000`

2. **Start the Frontend Application**
   ```bash
   cd frontend
   npm start
   ```
   The app will run on `http://localhost:3000`

3. **Start the Admin Panel**
   ```bash
   cd admin
   npm run dev
   ```
   The admin panel will run on `http://localhost:5173`

### Production Build

1. **Build Frontend**
   ```bash
   cd frontend
   npm run build
   ```

2. **Build Admin Panel**
   ```bash
   cd admin
   npm run build
   ```

## 🔌 API Endpoints

### Product Endpoints
- `GET /allproducts` - Get all products
- `POST /addproduct` - Add a new product (Admin)
- `POST /removeproduct` - Remove a product (Admin)
- `POST /upload` - Upload product image

### User Endpoints
- `POST /signup` - User registration
- `POST /login` - User login
- `POST /addtocart` - Add item to cart
- `POST /removefromcart` - Remove item from cart
- `POST /getcart` - Get user's cart

### Static Files
- `GET /images/:filename` - Access uploaded product images

## 🛒 Application Features

### Product Management
- Dynamic product catalog with categories
- Image upload and storage
- Product availability tracking
- Price management (old/new prices)

### User Authentication
- JWT-based authentication
- Secure password handling
- User cart persistence
- Session management

### Shopping Cart
- Add/remove items
- Quantity management
- Cart persistence across sessions
- Real-time cart updates

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 📞 Support

For support and questions, please contact any of the team members listed above.

---

**Happy Shopping! 🛍️** 