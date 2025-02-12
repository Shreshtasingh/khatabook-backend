

# **Khatabook Backend**  

A backend service for managing business transactions, customers, and financial records, built with **Node.js, Express.js, and MongoDB**.
This project is part of the **Khatabook** system, designed to help businesses track their financial transactions efficiently.  

## **Table of Contents**  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Project Structure](#project-structure)  
- [Installation](#installation)  
- [Environment Variables](#environment-variables)  
- [Running the Project](#running-the-project)  
- [API Endpoints](#api-endpoints)  
- [Contributing](#contributing)  
- [License](#license)  

---

## **Features**  
✅ User authentication and authorization  
✅ CRUD operations for customers and transactions  
✅ Secure password hashing using **bcryptjs**  
✅ Data storage with **MongoDB** and **Mongoose ORM**  
✅ API endpoints following **RESTful principles**  
✅ JWT-based authentication for security  

---

## **Technologies Used**  

| Technology  | Description  |
|-------------|-------------|
| **Node.js**  | JavaScript runtime for backend  |
| **Express.js**  | Web framework for building RESTful APIs  |
| **MongoDB**  | NoSQL database for storing user and transaction data  |
| **Mongoose**  | ODM (Object Data Modeling) for MongoDB  |
| **JWT (JSON Web Token)**  | Secure authentication and session management  |
| **bcryptjs**  | Hashing library for securing user passwords  |
| **dotenv**  | Environment variable management  |

---

## **Project Structure**  

```
khatabook-backend/
│── controllers/             # Business logic and request handling
│── models/                  # Mongoose schemas (User, Transaction, etc.)
│── routes/                  # API endpoints for user and transaction management
│── middleware/              # Authentication and authorization logic
│── config/                  # Database connection and environment setup
│── server.js                # Main server file (entry point)
│── package.json             # Dependencies and scripts
│── .env                     # Environment variables (ignored in Git)
│── README.md                # Project documentation
```

---

## **Installation**  

### **Prerequisites**  
Ensure you have the following installed on your system:  
- [Node.js](https://nodejs.org/)  
- [MongoDB](https://www.mongodb.com/)  
- [Git](https://git-scm.com/)  

### **Clone the Repository**  
```bash
git clone https://github.com/Shreshtasingh/khatabook-backend.git
```
```bash
cd khatabook-backend
```

### **Install Dependencies**  
```bash
npm install
```

---

## **Environment Variables**  

Create a `.env` file in the root directory and add the following values:  
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/khatabook
JWT_SECRET=your_secret_key
```

> Replace `your_secret_key` with a strong random string.

---

## **Running the Project**  

### **Start MongoDB** (if not running already)  
```bash
mongod
```

### **Run the server**  
```bash
npm start
```

The server will start on `http://localhost:5000`

---

## **API Endpoints**  

### **User Authentication**  
| Method | Endpoint | Description |
|--------|---------|-------------|
| `POST` | `/api/auth/register` | Register a new user |
| `POST` | `/api/auth/login` | Login and receive a JWT token |

### **Customer Management**  
| Method | Endpoint | Description |
|--------|---------|-------------|
| `GET` | `/api/customers` | Get all customers |
| `POST` | `/api/customers` | Add a new customer |
| `PUT` | `/api/customers/:id` | Update customer details |
| `DELETE` | `/api/customers/:id` | Remove a customer |

### **Transaction Management**  
| Method | Endpoint | Description |
|--------|---------|-------------|
| `GET` | `/api/transactions` | Get all transactions |
| `POST` | `/api/transactions` | Add a new transaction |
| `PUT` | `/api/transactions/:id` | Update transaction details |
| `DELETE` | `/api/transactions/:id` | Delete a transaction |

> All protected routes require a **JWT token** in the `Authorization` header.

---

## **Contributing**  

Contributions are welcome! Follow these steps:  
1. **Fork** this repository.  
2. **Create** a new branch:  
   ```bash
   git checkout -b feature-name
   ```
3. **Make your changes** and commit:  
   ```bash
   git commit -m "Added new feature"
   ```
4. **Push** to your branch:  
   ```bash
   git push origin feature-name
   ```
5. **Open a Pull Request** and wait for approval.  

---

## **License**  

📜 This project is open-source and available under the **MIT License**.![WhatsApp Image 2025-02-12 at 22 52 57_7ae64efd](https://github.com/user-attachments/assets/263e0f59-bdfd-4e2b-8f21-adc59724c966)
![WhatsApp Image 2025-02-12 at 22 52 58_10a933ba](https://github.com/user-attachments/assets/004a62dd-5fc3-4c97-b69c-a47500ec5817)
![WhatsApp Image 2025-02-12 at 22 52 58_b28f9f8e](https://github.com/user-attachments/assets/95e3b419-2208-416a-b8dc-415819dae5af)
![WhatsApp Image 2025-02-12 at 22 52 58_b28f9f8e](https://github.com/user-attachments/assets/0e7c717f-681e-4445-91c2-670177a2eb4c)
