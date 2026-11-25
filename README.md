# E-Commerce Website

A web-based E-Commerce application developed using Python Flask and MySQL. The application allows users to browse products, manage their shopping cart, place orders and make payments. It also includes an admin section to manage products, users and orders.

## Features

### User Features
- User registration and login
- Secure password hashing using Bcrypt
- Browse products and product categories
- View individual product details
- Add products to shopping cart
- Update product quantities and remove cart items
- Checkout and place orders
- Cash on Delivery (COD)
- Online payment integration using Razorpay
- View order history and order details
- View and update user profile
- Generate and view order invoices

### Admin Features
- Admin login and dashboard
- View total products, users, categories and orders
- Add new products
- Update existing product details
- Upload product images
- Manage product categories
- View and manage orders
- View registered users

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend development |
| Flask | Web framework |
| MySQL | Database management |
| HTML | Web page structure |
| CSS | Styling |
| JavaScript | Frontend functionality |
| Jinja2 | Template rendering |
| Bcrypt | Password hashing |
| Razorpay | Online payment integration |
| Python-dotenv | Environment configuration |

## Project Structure

```text
E-commerce-website/
│
├── database/
│   ├── connection.py
│   ├── tables.py
│   └── queries.py
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   ├── admin/
│   ├── user/
│   └── base.html
│
├── app.py
├── main.py
├── utils.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Manusha-M/E-commerce-website.git
```

### 2. Navigate to the Project Directory

```bash
cd E-commerce-website
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows**
```bash
venv\Scripts\activate
```

**Linux / macOS**
```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure MySQL Database

- Install and start MySQL.
- Create a database named `ecommerce3`.
- Configure your database connection details.
- Ensure the database connection settings are available through environment variables.

### 6. Configure Environment Variables

Create a `.env` file in the root directory:

```env
SECRET_KEY=your_secret_key
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=ecommerce3

RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Make sure your Python application reads these environment variables.

### 7. Run the Application

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:5000/
```

## Payment Integration

The application integrates Razorpay for online payments.

It supports:
- Razorpay order creation
- Payment processing
- Payment signature verification
- Payment success and failure handling

Cash on Delivery is also available as a payment option.

## Database

The application uses MySQL to store and manage:

- User information
- Product details
- Shopping cart items
- Customer orders
- Order details
- Payment information

## Future Improvements

- Product search and advanced filtering
- Product ratings and reviews
- Email notifications for orders
- Improved responsive UI
- Order tracking
- Deployment to a cloud platform

## Author

**Manusha Manne**

- GitHub: [Manusha-M](https://github.com/Manusha-M)
- LinkedIn: [Manusha Manne](https://www.linkedin.com/in/manushamanne)

---

If you find this project useful, feel free to explore the repository and share your feedback.
