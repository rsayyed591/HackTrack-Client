<div align="center">

# 🚀 HackTrack

### Modern Hackathon Management Platform

*Formerly known as **Hack Management***

A centralized platform for managing hackathons—from participant registration to final judging and live leaderboards.

[![Live Demo](https://img.shields.io/badge/Live-Demo-success?logo=vercel)](https://err404-manager.vercel.app)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)](#)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite)](#)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css)](#)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

🌐 **Live:** https://err404-manager.vercel.app

</div>

---

# 📖 Overview

HackTrack is a role-based hackathon management platform designed to streamline every stage of a hackathon. It provides dedicated portals for Participants, Judges, Admins, and Super Admins, enabling organizers to efficiently manage registrations, team formation, QR-based check-ins, judging, and real-time leaderboard generation from a single dashboard.

Instead of relying on spreadsheets and multiple disconnected tools, HackTrack centralizes the entire event lifecycle into one modern web application.

---

# ✨ Features

## 👨‍💻 Participant Portal

- Registration & Authentication
- Team Formation
- QR Check-in
- Food QR Verification
- Certificate Access
- Photo Uploads
- Assigned Problem Statements

---

## ⚖️ Judge Portal

- Assigned Teams Dashboard
- Team Evaluation
- Score Submission
- Edit Previous Scores
- Feedback Management

---

## 🛠 Admin Portal

- Participant Management
- Team Management
- Bulk User Import
- QR Check-in Operations
- Food Distribution
- Dashboard Analytics

---

## 👑 Super Admin Portal

- Judge Assignment
- Problem Statement Allocation
- Team Monitoring
- Live Leaderboards
- Complete Event Administration

---

## 🔐 Authentication & Security

- Role-Based Access Control (RBAC)
- Protected Routes
- Secure Authentication
- Permission-based Navigation
- Route Guards for all user roles

---

# 🛠 Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | React 18 |
| Build Tool | Vite |
| Routing | React Router DOM |
| Styling | Tailwind CSS |
| State Management | Context API |
| HTTP Client | Axios |
| Backend | Node.js + Express |
| Database | MongoDB |
| Authentication | JWT |
| Deployment | Vercel |

---

# 🏗 Architecture

HackTrack follows a role-isolated architecture where each authenticated user is redirected to a dedicated workspace based on their permissions.

```
                    Login
                      │
          Authentication (JWT)
                      │
        ┌─────────────┼─────────────┐
        │             │             │
        ▼             ▼             ▼
 Participant      Judge         Admin
        │             │             │
        └─────────────┼─────────────┘
                      ▼
                 Super Admin
                      │
                      ▼
                 REST API Server
                      │
                      ▼
                  MongoDB
```

Route protection is enforced using custom route wrappers to prevent unauthorized access across all user roles.

---

# 🌐 Live Demo

🔗 https://err404-manager.vercel.app

---

# 🚀 Getting Started

## Prerequisites

- Node.js (v14 or higher)
- npm
- Running HackTrack Backend API

---

## Installation

Clone the repository

```bash
git clone https://github.com/rsayyed591/HackTrack-client.git

cd HackTrack-client
```

Install dependencies

```bash
npm install
```

Create environment file

```bash
cp .env.example .env
```

Configure

```env
VITE_API_BASE_URL=http://localhost:5000
```

Run the development server

```bash
npm run dev
```

---

# 📂 Project Structure

```
src/
│
├── components/
│   ├── AutoComplete.jsx
│   ├── Loader.jsx
│   ├── GoBackButton.jsx
│   └── ProtectedRoute.jsx
│
├── contexts/
│   └── AuthContext.jsx
│
├── pages/
│   ├── admin/
│   ├── auth/
│   ├── judge/
│   ├── participant/
│   └── superadmin/
│
├── services/
│   └── api.js
│
├── App.jsx
└── main.jsx
```

---

# ⚡ Performance

- Responsive UI
- Optimized API calls
- Protected client-side routing
- Context-based authentication
- Modular architecture
- Fast Vite builds

---

# 📸 Screenshots

> Add screenshots of:

- Login Page
- Participant Dashboard
- Admin Dashboard
- Judge Dashboard
- Super Admin Dashboard
- Leaderboard
- QR Check-in
- Team Management

---

# 🗺 Roadmap

- [ ] Route-based code splitting
- [ ] WebSocket-powered live leaderboards
- [ ] Push notifications
- [ ] Dark Mode
- [ ] Export reports (PDF/Excel)
- [ ] Analytics Dashboard
- [ ] Email Notifications
- [ ] Multi-event support

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository

2. Create a feature branch

```bash
git checkout -b feature/amazing-feature
```

3. Commit changes

```bash
git commit -m "feat: add amazing feature"
```

4. Push changes

```bash
git push origin feature/amazing-feature
```

5. Open a Pull Request

---

# 👨‍💻 Developers

## Frontend

**Rehan Sayyed**

- GitHub: https://github.com/rsayyed591
- LinkedIn: https://linkedin.com/in/rehan42
- Portfolio: https://iamrehan.dev

---

## Backend

**Rehan Shah**

GitHub:
https://github.com/rehannn03

---

# 🙏 Acknowledgements

Special thanks to everyone who contributed to HackTrack.

Built using:

- React
- Vite
- Tailwind CSS
- Node.js
- Express
- MongoDB
- Vercel

---

# 📄 License

Distributed under the MIT License.

See the **LICENSE** file for more information.

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

Made with ❤️ by **Rehan Sayyed**

</div>
