## 📌 Overview
LapShop is a fully integrated e-commerce platform for selling laptops, allowing users to browse products, add them to the cart, create a new account, log in, and manage orders through the **admin panel**. It also supports **ASP.NET Identity** for security and role management.

## 🚀 DATABASE DESIGN

> ![Hosted Image](https://github.com/SE-ZEYAD/E-Commerce-Platform/blob/main/lap-shop.png)

## 🚀 Features
- **Category Management:** View, create, edit, and delete categories.
- **Product Management:** View, add, edit, and delete products.
- **Order Management:** Track orders and their status.
- **User Registration & Login:** Supports user authentication using **ASP.NET Identity**.
- **Roles & Permissions:** Assign roles to users (Admin, User) using **ASP.NET Identity**.
- **Cart Management:** Add products to the cart and complete orders.
- **API Integration:** Provides an API for easy data handling.

## 🔐 Security & Authentication
The project uses **ASP.NET Identity** for user and role management:
- **Regular User (User):** Can browse products, add to cart, and place orders.
- **Administrator (Admin):** Has full access to manage products, categories, and orders.

### User Registration
- User data is stored in **SQL Server** using **Entity Framework**.
- Supports **password encryption and security**.

### Role Management
- When a user registers, they are automatically assigned the **User** role.
- Admins can manage user roles via the **admin panel**.

---

## 🌐 API Endpoints
The project supports an API for interacting with data:

### 🛒 Products API
| Endpoint               | Method | Description          |
|------------------------|--------|----------------------|
| `/api/products`       | GET    | Retrieve all products |
| `/api/products/{id}`  | GET    | Retrieve a specific product |
| `/api/products`       | POST   | Add a new product |
| `/api/products/{id}`  | PUT    | Update a product |
| `/api/products/{id}`  | DELETE | Delete a product |

### 🛍️ Orders API
| Endpoint               | Method | Description          |
|------------------------|--------|----------------------|
| `/api/orders`         | GET    | Retrieve all orders |
| `/api/orders/{id}`    | GET    | Retrieve a specific order |
| `/api/orders`         | POST   | Create a new order |

---

## 🔧 Installation & Setup

### 💻 Prerequisites
- .NET 6.0 or later
- SQL Server
- Visual Studio 2022

### ⬇️ Clone the Repository
```bash
git clone https://github.com/yourusername/LapShop.git
cd LapShop
```

### 📦 Install Dependencies
```bash
dotnet restore
```

### 🛠️ Configure Database
1. Ensure the **Connection String** is set correctly in `appsettings.json`.
2. Create the database using Entity Framework:
```bash
dotnet ef database update
```

### 🚀 Run the Application
```bash
dotnet run
```

Open your browser and navigate to `http://localhost:5000` to explore the website.

---

## 📢 Contribution
If you’d like to contribute:
1. **Fork** the repository.
2. Create a **new branch** for your feature.
3. **Commit** and **push** your changes.
4. Create a **Pull Request**.

---

## 📜 License
This project is open-source and available under the **MIT License**.

---
