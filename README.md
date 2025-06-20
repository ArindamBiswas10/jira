# 🧩 Jira Clone — Project & Issue Tracking System

[![Next.js](https://img.shields.io/badge/Next.js-000?logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-38b2ac?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A high-performance, full-stack **Jira Clone** that replicates core functionalities of Atlassian Jira — built for teams to manage projects, track bugs, and streamline workflows with a modern, responsive UI.

> 🚀 Built with performance, scalability, and developer experience in mind.

---

## 📌 Demo

🔗 **Live Demo:** [your-demo-link.vercel.app](https://your-demo-link.vercel.app)  
📽️ **Video Walkthrough:** [Watch here](https://your-loom-or-youtube-demo.com)

---

## 🛠️ Tech Stack

| Layer         | Technology                                  |
| ------------- | ------------------------------------------- |
| Frontend      | Next.js, React, TypeScript, Tailwind CSS    |
| Backend       | Node.js, Express.js                         |
| Database      | PostgreSQL                                  |
| Auth          | NextAuth.js / JWT                           |
| Drag & Drop   | `@dnd-kit` or `react-beautiful-dnd`         |
| State Mgmt    | Zustand / Redux Toolkit                     |
| Deployment    | Vercel (Frontend), Railway / Render (API)   |

---

## ✨ Features

- 🔐 **Secure Authentication** — Login/Register with session protection
- 📁 **Project Board** — Create boards with columns like To Do, In Progress, Done
- 🧩 **Task Management** — Create, update, delete issues with priority, labels, due dates
- 🧲 **Drag & Drop** — Reorder tasks within and across columns
- 🧠 **Global State Management** — Zustand or Redux for smooth performance
- 🔍 **Advanced Filters** — Filter issues by status, assignee, or priority
- 🧑‍🤝‍🧑 **Team Collaboration Ready** — (Optional) Assign users to issues
- 📱 **Fully Responsive** — Optimized for mobile, tablet, and desktop
- 🧪 **Scalable Architecture** — Modular structure for easy scaling and maintenance

## 📂 Project Structure

jira-clone/
├── backend/ # Express + MongoDB API
│ ├── models/
│ ├── routes/
│ └── controllers/
├── frontend/ # Next.js + Tailwind client
│ ├── components/
│ ├── pages/
│ ├── hooks/
│ └── utils/
└── README.md


---

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/arindambiswas/jira-clone.git
cd jira-clone

### 2. 🛡️ Setup Environment Variables

Create `.env` files in both the **frontend** and **backend** directories to securely store configuration details.

#### 🔐 Frontend (`frontend/.env.local`)

```env
NEXT_PUBLIC_API_URL=http://localhost:5000
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000

Replace your_nextauth_secret with a secure, random string. You can generate one using openssl rand -base64 32.

### 🔐 Backend (backend/.env)
env
Copy
Edit
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
Make sure MongoDB is running locally or use a cloud service like MongoDB Atlas and replace your_mongodb_connection_string accordingly.