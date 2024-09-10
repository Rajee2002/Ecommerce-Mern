## MERN E-commerce Website

**MERN Ecommerce** is a full-stack application created to improve your online buying experience. It's built on the MERN stack (MongoDB, Express.js, React, and Node.js), with Redux Toolkit for efficient state management and Material UI for a clean, user-friendly interface. This project provides a strong platform for both users and administrators, complete with necessary features for a smooth experience.

![ecommerce-homepage](https://github.com/Rajee2002/Ecommerce-Mern/blob/main/frontend/src/assets/images/front.png?raw=true)
![ecommerce-banner](https://github.com/Rajee2002/Ecommerce-Mern/blob/main/frontend/src/assets/images/banner3.jpg?raw=true)


# **Features**

### **User:**
- **Product Reviews:** Users can Write, edit, and delete reviews. It will instantly update the ratings and star percentages.
  
- **Wishlist:** Users can add, remove, and annotate products with personalized notes.
  
- **Order Management:** Users can create new orders and view order history.
  
- **Profile Management:** Users can manage email, username, and multiple choice of address locations.
  
- **Shopping Cart:** Users can add products to their carts, adjust quantities, and view subtotals.

### **Admin:**
- **Product Management:** Admin can addd, edit, delete, and soft-delete products. They can also manage product attributes like name and stock.
  
- **Order Management:** Admin can view and update order details and status as per requirements.

### **Security & User Experience:**
- **Secure Authentication:** Login, signup, OTP verification, password reset, and logout.

- **Intuitive Interface:** Powered by Material UI for a visually appealing and user-friendly experience.

# **Project Setup**

### Prerequisites
- Node.js
- MongoDB

### Clone the project

```bash
  git clone https://github.com/Rajee2002/Ecommerce-Mern.git
```

### Navigate to the project directory

```bash
  cd Ecommenrce-mern
```

### Install dependencies for frontend and backend separately

Install frontend dependencies
```bash
cd frontend
npm install
```

Install backend dependencies

```bash
cd backend
npm install
```

### Environment Variables
**Backend**
- Create a `.env` file in the `backend` directory.
- Add the following variables with appropriate values
```bash
MONGO_URI="mongodb://localhost:27017/your-database-name"

ORIGIN="http://localhost:3000"

EMAIL="your-email@example.com"
PASSWORD="your-email-password"

LOGIN_TOKEN_EXPIRATION="30d"  # Days
OTP_EXPIRATION_TIME="120000"  # Milliseconds
PASSWORD_RESET_TOKEN_EXPIRATION="2m"  # Minutes
COOKIE_EXPIRATION_DAYS="30"    # Days

# Secret key for jwt security
SECRET_KEY="your-secret-key"

PRODUCTION="false" # Initially set to false for development
```

**Frontend**
- Create a `.env` file in the `frontend` directory
- Add the following variable:
```bash

REACT_APP_BASE_URL="http://localhost:8000" 
```

### Data seeding
- **Get started quickly with pre-populated data**: Populate your database with sample users, products, reviews, and carts.

**Steps**:
- Open a new terminal window.
- Navigate to the `backend` directory: `cd backend`
- Run the seeding script: `npm run seed`

### Running Development Servers

**Important:**

- **Nodemon required**: Ensure you have `nodemon` installed globally to run the backend development servers using `npm run dev`. You can install it globally using `npm install -g nodemon`.

#### Start the backend server
- Navigate to the `backend` directory: `cd backend`
- Start the server: `npm run dev` (or npm start)
- You should see a message indicating the server is running, usually on port 8000.
     
#### Start the frontend server:
- Navigate to the `frontend` directory: `cd frontend`
- Start the server: `npm start`
- You should see a message indicating the server is running, usually on port 3000.

### Accessing the Application
Once both servers are running, you can access them at the following URL's:
- Backend: http://localhost:8000
- Frontend: http://localhost:3000
