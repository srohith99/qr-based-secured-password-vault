# QR-Based Secured Password Vault

A **security-centric password vault** designed to demonstrate real-world cybersecurity practices such as **QR-based authentication, encrypted password storage, session hardening, anti-screenshot protection, location-based access tracking, and security monitoring**.

This project focuses on **how modern password managers protect sensitive data**, not just basic CRUD functionality.

## Project Overview

The **QR-Based Secured Password Vault** is a web-based application that allows users to securely store and manage passwords using **multi-layer security controls**.

Instead of exposing passwords directly, the system enforces **secondary authentication (QR-based)**, **time-limited password reveal**, and **active monitoring of suspicious user actions**.  
If risky behavior is detected (screenshots, snipping tools, tab switching, multiple faces, etc.), the vault **automatically locks itself**.

The project is built as a **cybersecurity-focused academic project**, inspired by real-world password managers and Zero-Trust principles.


## Key Features

### Authentication & Access Control
- QR-based login authentication
- Mobile-assisted verification
- Polling-based QR status validation
- Secure session initialization and termination

### Password Management
- Add encrypted password entries
- Secure password reveal with secondary verification
- Time-limited password visibility
- Soft delete and restore support
- Permanent deletion option
- No plaintext password storage

### Active Security Protections
- Screenshot & snipping-tool detection
- PrintScreen and print-dialog blocking
- Tab-switch and visibility change detection
- Panic / emergency auto-lock
- Webcam-based detection hooks (face / presence)

### Monitoring & Transparency
- Location-based last access tracking (with user permission)
- Session summaries with IST timestamps
- Security event logging
- Downloadable session reports

### Security Utilities
- Password strength analyzer
- Breach checker for compromised credentials
- Security dashboard & logs


##  Security Concepts Implemented

- Encryption at rest (AES-based)
- Zero-Trust inspired access model
- Least-privilege principle
- Time-bound secret exposure
- Session hardening & token invalidation
- Shoulder-surfing mitigation
- Privacy-aware location tracking
- Defensive UI/UX design

## 🛠 Tech Stack

- **Backend:** PHP  
- **Database:** MongoDB  
- **Frontend:** HTML, CSS, JavaScript  
- **AI / Detection:** face-api.js  
- **QR Authentication:** PHP + JavaScript  
- **Maps:** OpenStreetMap  
- **Client Security:** Browser Security APIs  

---

## ⚙️ Setup Instructions


Clone the repository:
   ```bash
   git clone https://github.com/srohith99/qr-based-secured-password-vault.git
```

setup:
  database_and_environment:
    - update_mongodb_credentials_in_configuration_files
    - ensure_no_secrets_are_hard_coded_before_deployment

  dependencies:
    - run: composer install
      note: install_only_if_dependencies_are_required

  server:
    supported_servers:
      - XAMPP
      - WAMP
      - LAMP
      - hosted_environment

  access:
    url: http://localhost/qr-based-secured-password-vault/



