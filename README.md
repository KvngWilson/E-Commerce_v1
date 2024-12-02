# E-Commerce_v1

E-Commerce Platform

A full-stack e-commerce application built using Django (backend) and React.js (frontend). This application supports user authentication, product management, order handling, and integration with the Paystack payment gateway. It is designed for scalability and provides an intuitive user experience with advanced features.
Table of Contents

    Features
    Technologies
    Installation
        Backend
        Frontend
    Environment Variables
    Usage
    Testing
    License

Features
Frontend

    Responsive UI with React.js.
    Advanced state management using Redux.
    User authentication (login, registration, and logout).
    Product search, filtering, and sorting.
    Shopping cart management.
    Payment integration with Paystack.
    Notifications using React Toastify.

Backend

    RESTful APIs built with Django REST Framework.
    Secure authentication with custom user models and token-based authentication.
    PostgreSQL database support.
    Webhook support for Paystack payment validation.
    Scalable structure with modular apps (users, products, orders).

Technologies
Frontend

    React.js
    Redux Toolkit
    Axios
    SCSS (Sass)
    React Router
    React Toastify

Backend

    Python
    Django
    Django REST Framework
    PostgreSQL
    Paystack API Integration

Installation
Backend

    Clone the repository:

git clone https://github.com/KvngWilson/E-Commerce_v1.git
cd E-Commerce_v1/backend

Set up a virtual environment:

python3 -m venv venv
source venv/bin/activate

#Install dependencies:

pip install -r requirements.txt

Apply migrations:

python manage.py migrate

Start the development server:

    python manage.py runserver

Frontend

    Navigate to the frontend directory:

cd ecommerce-platform/frontend

Install dependencies:

npm install

Start the development server:

    npm start

Environment Variables

Create an .env file in both the backend and frontend directories with the following variables:
Backend (.env)

SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_HOST=127.0.0.1
DB_PORT=5432
PAYSTACK_PUBLIC_KEY=your_paystack_public_key
PAYSTACK_SECRET_KEY=your_paystack_secret_key
CORS_ALLOWED_ORIGINS=http://localhost:3000

Frontend (.env)

REACT_APP_API_BASE_URL=http://127.0.0.1:8000/api
REACT_APP_PAYSTACK_PUBLIC_KEY=your_paystack_public_key

Usage

    Navigate to the frontend in your browser:
        Default URL: http://localhost:3000

    Available Features:
        Guest Users: Browse products, search, and filter.
        Registered Users: Add items to the cart, checkout, and view order history.

Testing
Backend

Run tests for the backend:

python manage.py test

Frontend

Run tests for the frontend:

npm test

License

This project is licensed under the MIT License.
Contributions

Contributions are welcome! If you'd like to contribute, please:

    Fork the repository.
    Create a feature branch.
    Submit a pull request.
