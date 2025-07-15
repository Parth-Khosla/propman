# 🏢 PropMan – Property Management SaaS Platform

**PropMan** is a full-stack SaaS-based web application designed to streamline property management operations for property managers. It provides tools for managing properties, tenants, staff, units, and complaint resolution – all in one centralized dashboard.

---

## 🚀 Technologies Used

### 🧠 Backend
- **Python** (FastAPI) – High-performance, asynchronous API backend
- **MySQL** – Relational database for structured data
- **JWT Authentication** – Secure, token-based user authentication
- **Email-based OTP** – For secure verification during login and registration

### 🎨 Frontend
- **React.js** – Dynamic and modern frontend SPA framework
- **TailwindCSS / Material UI** – For responsive and aesthetic UI components

### ☁️ DevOps / Infrastructure
- **Docker** – Containerized deployment
- **Nginx** – Reverse proxy and static file server
- **SMTP Provider** – For sending OTP emails (e.g., SendGrid, Brevo)

---

## 🌟 Key Features

### 🔐 Authentication & Security
- OTP-based Email Verification (Signup/Login/Forgot Password)
- JWT-based session management
- Role-based access: Property Manager, Tenant, Staff

### 🏠 Property Management
- Register and manage multiple properties
- Define units per property with details like area, type, charges, etc.
- Track unit availability and tenant history

### 👤 Tenant Management
- Property managers can onboard tenants
- Tenants complete onboarding via OTP link
- Allocate units and lease details
- View tenant profiles and agreements

### 🧾 Complaint Management
- Tenants can raise complaints with images and priority level
- Auto-notification to property manager
- Assign complaints to staff (electrician, plumber, etc.)
- Staff updates status and resolution with comments/photos

### 👨‍🔧 Staff Management
- Onboard maintenance staff with profile and shift details
- Dashboard for staff to view and resolve complaints

### 📊 Dashboards & Reports
- Property Manager Dashboard:
  - Total Properties
  - Total Tenants
  - Units Availability
  - Recent Complaints
- Tenant Dashboard:
  - Complaint summary
  - Personal property/unit info
- HTML-based reports (Tenants, Staff, Complaints)

---

## 📁 Project Structure

propman/
├── documents/
├── backend/ # FastAPI app with routers, models, and DB
├── frontend/ # React.js frontend app
├── docker-compose.yml # Dev environment with DB, API, frontend
└── README.md

## Backend Setup
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload

## Frontend Setup
cd frontend
npm install
npm run dev
# propman
