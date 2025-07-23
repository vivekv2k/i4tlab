# 📝 Task Manager Application# i4tlab

A full-stack task management application built with **Laravel (API)** as the backend and **React + Vite** as the frontend. It supports task creation, assignment, filtering, status updates, and user management.

## 🚀 Features

- Create, view, edit, and delete tasks
- Assign tasks to users
- Filter tasks by status or assigned user
- Paginated task listing
- SweetAlert modals for confirmation and alerts
- Reusable modal components
- Status update via dropdown (pending / completed)

- ---

## 🛠️ Tech Stack

### Backend
- Laravel 10+
- RESTful API with Resource Controllers
- MySQL / MariaDB
- Repository Pattern (SOLID principles)
- Seeder and Factory support

### Frontend
- React 19 with Vite
- Redux Toolkit for state management
- Tailwind CSS for UI
- SweetAlert2 for dialogs

---

## 📦 Installation

### Backend (Laravel)

```bash
cd backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve
-
```
please run db seeder 

###Ensure you have a database configured in .env.


cd frontend
npm install
npm run dev


The frontend runs at http://localhost:5173 by default.



📂 Folder Structure

Laravel

    app/Repositories – Task repository implementing interface

    app/Http/Controllers/Api/TaskController.php

    database/seeders/UserSeeder.php, TaskSeeder.php

React

    src/components/ – All UI components

    src/redux/ – Redux store and slices

    src/services/api.js – Axios config

    src/pages/TaskList.jsx – Main task listing page
