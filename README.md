# 🚀 HackTrack *(Formerly Hack Management)*

[![Live Demo](https://img.shields.io/badge/Vercel-Live-success?logo=vercel)](https://err404-manager.vercel.app)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)](#)
[![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite)](#)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> **"Turning hackathon chaos into organized innovation."**

HackTrack is a modern, role-based hackathon management platform that streamlines everything from participant registration and QR check-ins to judging, team management, and live leaderboards—all from a single dashboard.

---

## 🌐 Live Demo

**Production:** https://err404-manager.vercel.app

---

## 📖 About

HackTrack was built to simplify the logistics of organizing hackathons. Instead of juggling spreadsheets, forms, and multiple communication channels, organizers can manage the complete event lifecycle through one centralized application.

The platform provides dedicated portals for **Participants**, **Judges**, **Admins**, and **Super Admins**, ensuring each role has access only to the tools and information they need.

Whether you're running a university hackathon or a large-scale coding competition, HackTrack helps organizers focus on the event—not the operations.

---

## ✨ Features

### 👨‍💻 Participant Portal

* Secure authentication
* Team formation
* QR-based event check-in
* Food distribution QR
* Assigned problem statements
* Certificate access
* Photo uploads

### ⚖️ Judge Portal

* Assigned team dashboard
* Score submission
* Edit evaluations
* Feedback management
* Previous submissions

### 🛠 Admin Portal

* Participant management
* Team management
* Bulk user import
* QR check-in operations
* Food distribution management
* Dashboard overview

### 👑 Super Admin Portal

* Judge assignment
* Problem statement allocation
* Team management
* Live leaderboard
* User management
* Complete event administration

### 🔐 Security

* Role-Based Access Control (RBAC)
* Protected Routes
* JWT Authentication
* Permission-based navigation
* Secure session management

---

## 🛠 Technology Stack

| Category             | Technology        |
| -------------------- | ----------------- |
| **Frontend**         | React 18          |
| **Build Tool**       | Vite              |
| **Routing**          | React Router DOM  |
| **Styling**          | Tailwind CSS      |
| **State Management** | Context API       |
| **HTTP Client**      | Axios             |
| **Backend**          | Node.js + Express |
| **Database**         | MongoDB           |
| **Deployment**       | Vercel            |

---

## 🏗 Architecture

The frontend follows a role-based architecture where every authenticated user is redirected to a dedicated workspace based on their permissions.

Authentication is managed through a centralized **AuthContext**, while route protection is enforced using custom wrapper components such as:

* `ProtectedRoute`
* `AdminRoute`
* `JudgeRoute`
* `SuperAdminRoute`

This ensures users cannot access routes or interfaces outside their assigned role.

---

## 📂 Project Structure

```text
src/
├── components/
│   ├── AutoComplete.jsx
│   ├── GoBackButton.jsx
│   ├── Loader.jsx
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
├── main.jsx
└── index.css
```

---

## 🚀 Getting Started

### Prerequisites

* Node.js **14+**
* npm
* Running HackTrack Backend API

### Installation

Clone the repository.

```bash
git clone https://github.com/rsayyed591/HackTrack-client.git

cd HackTrack-client
```

Install dependencies.

```bash
npm install
```

Create an environment file.

```bash
cp .env.example .env
```

Configure your environment variables.

```env
VITE_API_BASE_URL=http://localhost:5000
```

Start the development server.

```bash
npm run dev
```

---

## ⚙️ Environment Variables

| Variable            | Description          |
| ------------------- | -------------------- |
| `VITE_API_BASE_URL` | Backend API base URL |

---

## 🗺 Roadmap

* [ ] Route-based code splitting
* [ ] Live leaderboard updates using WebSockets
* [ ] Event analytics dashboard
* [ ] Email notifications
* [ ] Multi-event support
* [ ] Dark mode
* [ ] Export reports
* [ ] Docker deployment

---

## 🤝 Contributing

Contributions are always welcome.

1. Fork the repository.
2. Create a feature branch.

```bash
git checkout -b feature/amazing-feature
```

3. Commit your changes.

```bash
git commit -m "feat: add amazing feature"
```

4. Push your branch.

```bash
git push origin feature/amazing-feature
```

5. Open a Pull Request.

---

## 🙏 Acknowledgements

Special thanks to **Rehan Shah** for designing and developing the backend architecture and APIs that power HackTrack.

**GitHub:** https://github.com/rehannn03

---

## 👨‍💻 Author

### Rehan Sayyed

* 🌐 Portfolio: https://iamrehan.dev
* GitHub: https://github.com/rsayyed591
* LinkedIn: https://linkedin.com/in/rehan42

---

<div align="center">

### ⭐ Enjoying HackTrack?

If you found this project useful, consider giving it a **star**.

Made with ❤️ by **Rehan Sayyed**

</div>
