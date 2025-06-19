# Assignment-1-WebAppSec
Assignment 1

# Laravel To-Do App with Enhanced Authentication & Profile Page

This is a Laravel-based To-Do App enhanced with:

## ✅ Features Added

### 🔐 Registration & Login Input Validation
- Implemented using Laravel **Form Request** classes.
- Fields validated using **regex** and built-in Laravel rules:
  - Name: only accepts A-Z, a-z using `regex:/^[A-Za-z ]+$/`
  - Email: required, must be valid and unique
  - Password: required, min 8 chars, confirmed

### 👤 User Profile Page
- Accessible only to authenticated users
- Editable fields:
  - Nickname
  - Email
  - Password (with confirmation)
  - Phone number
  - City
  - Avatar upload (JPEG/PNG)
- Avatar preview supported
- **Delete account** button (permanently deletes user)

### 📁 File Uploads
- Avatar files are stored in `storage/app/public/avatars`
- Symbolic link created via `php artisan storage:link`

---

## 📦 Installation Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
