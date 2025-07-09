# Software Requirements Specification (SRS)

## Project Name: PropMan  
**Prepared By:** Parth Khosla 
**Date:** 9th July 2025  

---

## 1. Introduction

### 1.1 Purpose
This document specifies the software requirements for **PropMan**, a SaaS-based property management platform. It enables property managers to manage properties, tenants, complaints, and staff efficiently.

### 1.2 Scope
PropMan will be developed using Python (API), MySQL (database), and ReactJS (frontend). It will include:
- Property manager registration and login
- Property and tenant management
- Complaint handling and staff assignment
- Tenant portal to view property and raise complaints

### 1.3 Definitions and Abbreviations

| Term | Description |
|------|-------------|
| SaaS | Software as a Service |
| API | Application Programming Interface |
| UI | User Interface |
| SRS | Software Requirements Specification |

### 1.4 References
- [ReactJS Documentation](https://reactjs.org/)
- [FastAPI Documentation](https://fastapi.tiangolo.com/)
- [MySQL Documentation](https://dev.mysql.com/doc/)

---

## 2. Overall Description

### 2.1 Product Perspective
PropMan is a web-based system to be hosted on the cloud and accessed via browsers.

### 2.2 Product Functions
- Register and manage properties and tenants
- Track tenant history
- Manage staff (electrician, plumber, etc.)
- Complaint management system
- Role-based dashboard for manager, tenant, and staff

### 2.3 User Classes

| User | Description |
|------|-------------|
| Property Manager | Manages all aspects of properties |
| Tenant | Can view property and raise complaints |
| Staff | Assigned to fix complaints |

### 2.4 Operating Environment
- Backend: Python 3.x (FastAPI/Flask)
- Frontend: ReactJS
- Database: MySQL
- Deployment: Cloud (e.g., AWS, Azure)
- Browsers: Chrome, Firefox, Safari, Edge

### 2.5 Design Constraints
- Use of RESTful APIs
- JWT/OAuth2-based authentication
- Responsive UI design

---

## 3. System Features

### 3.1 Property Manager Module
- Register/Login
- Add/Edit/Delete properties
- Manage tenants and view history
- Add/Edit/Delete staff
- Assign complaints to staff
- View all complaints and dashboards

### 3.2 Tenant Module
- Register/Login
- View property details
- Raise and track complaints

### 3.3 Complaint Management
- Complaint submission by tenant
- Assignment by manager
- Status updates by staff
- Notifications for updates

### 3.4 Staff Module
- View assigned complaints
- Update status and resolution notes

### 3.5 Admin Panel
- Central dashboard for manager
- Reports: complaint logs, tenant history
- Full CRUD capabilities

---

## 4. External Interface Requirements

### 4.1 User Interface
- Clean, responsive UI
- Role-based portals: manager, tenant, staff

### 4.2 API Interface
- RESTful endpoints for all operations
- JSON-based communication

### 4.3 Hardware Interface
- Not applicable

### 4.4 Software Interface
- MySQL database
- SMTP or transactional email provider (e.g., SendGrid, Brevo)
- Optional: Firebase for push notifications

---

## 5. Non-Functional Requirements

### 5.1 Performance
- API response time < 500ms
- Optimized DB queries

### 5.2 Security
- Encrypted data storage
- Role-based access control
- Data isolation per manager

### 5.3 Usability
- Mobile-friendly interface
- Easy navigation and dashboards

### 5.4 Maintainability
- Modular backend and frontend
- API versioning

### 5.5 Availability
- 99.9% uptime SLA
- Daily backups

---

## 6. Assumptions and Dependencies
- Users have internet access
- A valid email is required
- External services (email, notifications) are available

---

## 7. Future Enhancements
- Rent payment and invoice module
- Digital lease agreements
- In-app chat for tenants and staff
- Mobile app version for iOS and Android

---
