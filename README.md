# StudyNotion FullStack Major Project

A production-style MERN learning platform where students discover courses, instructors publish content, and authenticated users manage their learning from role-based dashboards.

![Build](https://img.shields.io/badge/build-Vite%20%2B%20Express-success?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Version](https://img.shields.io/badge/version-0.0.0-orange?style=flat-square)
![Language](https://img.shields.io/badge/language-JavaScript-yellow?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/dev0302/StudyNotion_FullStack-Major-Project?style=flat-square)

## 🖼️ Screenshots

### 🖥️ Desktop
![Desktop View](./assets/home-desktop.png)

### 📱 Mobile
![Mobile View](./assets/home-mobile.png)

> [!TIP]
> Screenshots are auto-captured from the live deployment.

## 📚 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [API Reference](#-api-reference)
- [Configuration](#-configuration)
- [Contributing](#-contributing)
- [License](#-license)

## 🔎 Overview

StudyNotion is a full-stack e-learning platform inspired by modern course marketplaces. It combines a Vite-powered React frontend with an Express/MongoDB backend to support public course discovery, account creation, OTP verification, password reset flows, course creation, course content management, enrollment, progress tracking, ratings, reviews, and profile management.

The project exists as a major MERN learning build: it demonstrates how a real-world course platform can be split into a responsive single-page application, a REST API, persistent MongoDB models, role-based authorization, media uploads, transactional email templates, and dashboard workflows for different user types.

The app is built for:

- Students who want to browse, enroll in, and track courses.
- Instructors who want to create courses, organize sections/subsections, and view dashboard analytics.
- Admin-style workflows such as protected contact retrieval and category/course management.

Key architectural choices include:

- Client-side routing with protected and open route wrappers.
- Redux Toolkit slices for auth, profile, cart, course-building, and view-course state.
- Centralized Axios API connector using `VITE_BASE_URL`.
- Backend route separation by domain: auth, profile, course, and payment.
- JWT authentication with cookie/header token support.
- Role guards for `Student`, `Instructor`, and `Admin`.
- Cloudinary-backed media upload helpers.
- Email delivery through Brevo templates.

> [!NOTE]
> Dashboard routes exist in the app, but they are protected by authentication. The README screenshots show the public live home page.

## ✨ Features

### Public Experience

- ✅ Responsive landing page with StudyNotion branding and course-focused hero content.
- ✅ Public routes for Home, About, Contact, Catalog, Course Details, Login, Signup, My Journey, Forgot Password, and Reset Password.
- ✅ Catalog dropdown and category-driven course browsing flow.
- ✅ Contact form backed by an API endpoint.
- ✅ Reusable UI components such as Navbar, Footer, CTA buttons, tabs, spinners, rating stars, and confirmation modals.

### Authentication & Accounts

- ✅ Student and instructor signup flow.
- ✅ OTP generation and verification support.
- ✅ Login with JWT token handling.
- ✅ Password reset token and password update flow.
- ✅ Authenticated profile retrieval and update APIs.
- ✅ Profile picture upload support.
- ✅ Account deletion endpoint.

### Student Workflows

- ✅ Enrolled courses dashboard route.
- ✅ Wishlist/cart-style course flow.
- ✅ Course purchase history route.
- ✅ Full course view route for lecture playback.
- ✅ Course progress update endpoint.
- ✅ Rating and review creation.

### Instructor Workflows

- ✅ Instructor dashboard route.
- ✅ Course creation flow with multi-step course builder.
- ✅ Course editing and deletion.
- ✅ Section and subsection creation, update, and deletion.
- ✅ Course thumbnail and lecture media upload support.
- ✅ Instructor course listing and analytics endpoint.

### Backend & Integrations
