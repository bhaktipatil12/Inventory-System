# Inventory Management System

A full-stack **Inventory Management System** built with **FastAPI, React, and PostgreSQL** for efficient inventory tracking, warehouse management, and stock operations. The application provides secure authentication, real-time inventory monitoring, comprehensive reporting, and an intuitive dashboard to streamline warehouse operations.

---

## Features

* JWT Authentication & Secure Authorization
* Dashboard with Real-Time Inventory Analytics
* Product & Category Management
* Multi-Warehouse Inventory Management
* Stock Receipts, Deliveries, Transfers & Adjustments
* Inventory Movement History & Audit Logs
* Low Stock Alerts
* Reports & Inventory Analytics
* Location-Based Stock Tracking
* Responsive Modern UI

---

## Tech Stack

### Backend

* FastAPI
* PostgreSQL
* SQLAlchemy
* Alembic
* JWT Authentication
* Pydantic

### Frontend

* React
* Vite
* Tailwind CSS
* React Router
* Axios
* Recharts

---

## Project Structure

```text
Inventory-System/
│
├── backend/
│   ├── app/
│   ├── alembic/
│   ├── requirements.txt
│   └── main.py
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

# Installation

## Clone Repository

```bash
git clone <repository-url>

cd Inventory-System
```

---

## Backend Setup

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

pip install -r requirements.txt
```

Create a `.env` file:

```env
DATABASE_URL=postgresql://username:password@localhost:5432/inventory_db
SECRET_KEY=your_secret_key
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30
```

Run migrations:

```bash
alembic upgrade head
```

Start the backend:

```bash
uvicorn app.main:app --reload
```

---

## Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

---

## API Documentation

After starting the backend:

* Swagger UI → `http://localhost:8000/docs`
* ReDoc → `http://localhost:8000/redoc`

---

## Main Modules

* Authentication
* Dashboard
* Product Management
* Category Management
* Warehouse Management
* Stock Operations
* Inventory Reports
* Movement History

---

## Security

* JWT Authentication
* Password Hashing (bcrypt)
* Protected API Routes
* Input Validation
* SQLAlchemy ORM Protection
* Environment-Based Configuration

---

## Future Enhancements

* Barcode & QR Code Support
* Email Notifications
* Docker Deployment
* Role-Based Permissions
* Export Reports (PDF & Excel)
* CI/CD Pipeline
* Redis Caching

---

## License

This project is licensed under the MIT License.

---

## Author

**Bhakti Patil**

B.Tech Computer Science Engineering (AI & ML)

GitHub: https://github.com/bhaktipatil12
