# 🔐 Secured Vault System

A **security-focused password vault** designed with real-world threat models in mind.  
This project goes beyond basic CRUD operations and demonstrates how modern password managers protect sensitive data using **encryption, secondary authentication, session hardening, and user-behavior monitoring**.

---

## 🚀 Overview

The Secured Vault System is a web-based password manager that emphasizes **defense-in-depth security**.  
Passwords are encrypted at rest, revealed only after secondary verification, and automatically hidden after a short time window.

The system actively monitors risky actions such as screenshots, print attempts, and abnormal session behavior, triggering an automatic lock when threats are detected.

This project was built as a **cybersecurity-oriented academic project** to explore practical implementations of secure authentication, access control, and session protection.

---

## ✨ Key Features

### 🔑 Authentication & Access Control
- QR-based authentication flow
- Secondary verification before password reveal
- Time-limited password visibility

### 🔐 Password Security
- Encrypted password storage (AES-based)
- Add and delete password entries securely
- No plaintext password storage

### 🛡️ Active Security Protections
- Screenshot & snipping tool detection
- PrintScreen and print-dialog blocking
- Auto-lock on suspicious behavior
- Panic mode for instant vault lock

### 📍 Monitoring & Transparency
- Location-based last access tracking (with user permission)
- IST-based session timestamps
- Session summary and activity reports

### 🔍 Security Utilities
- Password strength analyzer
- Breach checker for compromised credentials
- Deleted-password management

---

## 🧠 Security Concepts Implemented

- Encryption at rest
- Zero-Trust inspired access model
- Least privilege principle
- Time-bound secret exposure
- Session hardening
- Shoulder-surfing mitigation
- Privacy-aware location tracking

---

## 🛠 Tech Stack

- **Backend:** PHP  
- **Database:** MongoDB  
- **Frontend:** HTML, CSS, JavaScript  
- **Security & AI:** TensorFlow.js  
- **Maps:** OpenStreetMap  
- **Utilities:** QR authentication, browser security APIs  

---

## 📂 Project Structure (Simplified)

