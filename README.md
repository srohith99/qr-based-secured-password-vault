# QR - Based Secured Password Vault System

A **security-focused password vault** built to demonstrate real-world cybersecurity concepts such as encrypted storage, QR-based authentication, session hardening, and protection against shoulder surfing and unauthorized access.

This project goes beyond basic CRUD operations and focuses on **how modern password managers defend sensitive data**.

## Project Overview

The Secured Vault System is a web-based application that allows users to securely store and manage passwords.  
Instead of relying only on traditional credentials, the system introduces **QR-based authentication**, **time-limited password reveal**, and **active monitoring of risky user behavior**.

The vault automatically locks itself when suspicious actions (screenshots, print attempts, abnormal behavior) are detected, ensuring enhanced session security.

## Key Features

### Authentication
- QR-based login authentication
- Mobile-assisted verification
- Secure session initialization

### Password Management
- Add encrypted password entries
- Secure password deletion
- No plaintext password storage

### Active Security Controls
- Screenshot & snipping tool detection
- PrintScreen and print-dialog protection
- Panic / emergency auto-lock
- Session-based access control

### Monitoring & Reporting
- Location-based last access tracking (with user permission)
- Session summary and activity tracking
- Timestamp handling in IST

### Security Utilities
- Password strength analyzer
- Breach checker for compromised credentials
- Deleted password management

---

## Security Concepts Implemented

- Encryption at rest (AES-based)
- Zero-Trust inspired authentication
- Least privilege principle
- Time-limited secret exposure
- Session hardening
- Shoulder surfing mitigation
- Privacy-aware location tracking

## Tech Stack

- **Backend:** PHP  
- **Database:** MongoDB  
- **Frontend:** HTML, CSS, JavaScript  
- **Face Detection / AI:** face-api.js  
- **QR Authentication:** PHP + JS  
- **Client Security:** Browser Security APIs  


## 📂 Project Structure

/assets
├── add_password.php # Add new encrypted password
├── dashboard.php # User vault dashboard
├── db_connect.php # Database connection
├── generate_qr.php # Generate QR for authentication / reveal
├── get_descriptor.php # Fetch face descriptor
├── index.php # Entry point
├── login.php # User login
├── logout.php # Logout and session cleanup
├── register.php # User registration
├── register_face.php # Face registration
├── save_descriptor.php # Save face descriptor
└── verify_qr.php # Verify QR authentication

/css
└── stylesheets # Application styles

/js
├── antiCapture.js # Screenshot & snipping protection
└── face-api.min.js # Face detection library

/qrcodes
└── generated QR images # Temporary QR codes

---

## ⚙️ Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/secured-vault-system.git

2. Configure database connection:

    Update MongoDB credentials inside db_connect.php

3. Place the project in a PHP-supported server:

    XAMPP / WAMP / LAMP / Live Server

4. Open in browser:

    http://localhost/secured-vault-system/

