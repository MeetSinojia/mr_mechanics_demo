# 🚀 Vendor Management & Booking System

A full-stack mobile application built using Flutter (Frontend) & Golang (Backend), designed for vendor management, bookings, billing, inventory, notifications, and multilingual support.

## 🎥 Demo
[View Demo Screenshots](https://github.com/MeetSinojia/mr_mechanic_codebase/blob/main/demo/demo.md)

## 📑 Table of Contents
- 📌 Features
- 🛠 Tech Stack
- 📂 Project Structure
- 🚀 Setup & Installation
- 🌍 Localization & Multilingual Support
- 🛡 Security Measures
- 🎯 Future Enhancements

## 📌 Features

### 📂 Vendor Management
- ✔️ Vendor registration & authentication (JWT-based)
- ✔️ Vendor profile management
- ✔️ Business switching (for multiple shops)
- ✔️ Subscription & package management

### 📅 Booking & Billing Management
- ✔️ Create, update, delete, and fetch bookings
- ✔️ Generate invoices for bookings
- ✔️ Manage services & items in bookings
- ✔️ Mark bookings as pending or completed

### 📦 Inventory Management
- ✔️ Add, update, delete inventory items
- ✔️ Fetch inventory by business ID, category, item ID
- ✔️ Track low stock items & inventory quantity
- ✔️ Inventory logs & photos management

### 🔔 Notification Management
- ✔️ Fetch active notifications for vendors
- ✔️ Real-time updates on bookings, inventory & bills

### 🌍 Multilingual & Localization
- ✔️ Supports multiple languages (English, Hindi, etc.)
- ✔️ Flutter JSON-based localization

### 📊 Reports & Analytics
- ✔️ View business statistics & reports
- ✔️ Analyze performance based on bookings & inventory

### 🛡 Security & Performance Enhancements
- ✔️ JWT Authentication for secure access
- ✔️ Rate limiting middleware to prevent abuse
- ✔️ Role-Based Access Control (RBAC) for vendors & users
- ✔️ Centralized logging & error handling

## 🛠 Tech Stack

### Frontend (Mobile App - Flutter)
- **Framework:** Flutter
- **State Management:** Provider
- **Localization:** AppLocalizations, JSON-based translations
- **Networking:** HTTP
- **UI Components:** Custom widgets, ResponsiveUtils
- **Storage:** SharedPreferences (local storage)

### Backend (REST API - Golang)
- **Framework:** Gin (lightweight, fast HTTP web framework)
- **ORM:** GORM (SQL database interactions)
- **Authentication:** JWT-based token authentication
- **Middleware:** Rate limiting, Logging, Error handling
- **Database:** MySQL (Relational DB)

### Infrastructure & Hosting
- **Backend Hosting:** Render (Golang)
- **Database:** AWS RDS (MySQL)
- **Object Storage:** AWS S3 / Google Cloud Storage
- **Messaging & OTP:** MSG91 (for authentication)

### Main Tech Stack Features:
- **Flutter Framework:**
  - Cross-platform development for iOS and Android.
  - Use of StatelessWidget and StatefulWidget for UI components.
  - Custom widgets for modular and reusable UI components.
- **State Management:**
  - Provider package for state management.
  - Use of ChangeNotifier for notifying listeners about state changes.
- **Localization:**
  - Multilingual support using AppLocalizations.
  - JSON files for storing localized strings (e.g., en.json, hi.json).
- **Responsive Design:**
  - ResponsiveUtils for adaptive UI design.
  - Consistent use of responsive padding, sizing, and text styles.
- **Networking:**
  - Asynchronous data fetching using Future and async/await.
  - Error handling for network requests.
- **Dependency Injection:**
  - Use of Provider for dependency injection and state management.
- **Custom Themes:**
  - Custom color schemes using AppColors.
  - Consistent theming across the app.
- **Asset Management:**
  - Use of flutter_svg for SVG assets.
  - Organized asset management for images and icons.
- **Error Handling:**
  - Comprehensive error handling for network requests and state management.
- **Modular Architecture:**
  - Well-structured, scalable code organization.

## 📂 Project Structure

### Frontend (Flutter)
```
/lib
  /screens       # UI Screens
  /widgets       # Custom UI Components
  /services      # API Calls & Business Logic
  /models        # Data Models
  /localization  # JSON-based localization files
  /utils         # Responsive Design Helpers
```

### Backend (Golang)
```
/services       # Business Logic
/repository     # Database Queries
/controllers    # API Handlers
/middleware     # JWT, Rate Limiting, Logging
/models         # DB Models
/config         # App Configuration
/routes         # API Routing
```

## 🚀 Setup & Installation

### 📌 Prerequisites
- Flutter SDK installed
- Golang & MySQL installed
- Render / AWS RDS Setup

### 📌 Backend Setup (Golang)
```bash
git clone <repo-url>
cd backend
go mod tidy
go run main.go
```

### 📌 Frontend Setup (Flutter)
```bash
git clone <repo-url>
cd frontend
flutter pub get
flutter run
```

## 🌍 Localization & Multilingual Support
- ✔ Flutter JSON-based localization (en.json, hi.json)

Example JSON:
```json
{
  "booking_title": "My Bookings",
  "inventory_title": "Inventory Management"
}
```
```json
{
  "booking_title": "मेरी बुकिंग",
  "inventory_title": "इन्वेंट्री प्रबंधन"
}
```

## 🛡 Security Measures
- ✔ JWT Authentication for secure login
- ✔ Rate Limiting Middleware to prevent abuse
- ✔ RBAC (Role-Based Access Control)
- ✔ Centralized Logging & Error Handling

## 🎯 Future Enhancements
- 🔹 AI-based Recommendations for Inventory & Bookings
- 🔹 Push Notifications for Updates
- 🔹 Offline Mode for Flutter App
- 🔹 GraphQL Support for APIs

