# 🏢 HostelMate: Pro Advanced Hostel Management Platform

A modern, enterprise-grade Hostel Management System built with **React Native (Expo)** on the frontend and **Node.js (Express & Sequelize)** on the backend. Designed with a custom **Cherry & Alabaster** UI/UX.

---

## 🌟 Modules & Capabilities

1. **Student Records Management**: Directory with enrollment, roll numbers, guardian contacts, room/bed assignment, and fee tracking.
2. **Room Allocation**: Structured bed-level allocation (`Bed A`, `Bed B`, `Bed C`), visual occupancy grid, floor filtering, and maintenance status control.
3. **Complaint Tracking**: Priorities (`Urgent`, `High`, `Normal`, `Low`), categories, lifecycle statuses (`Pending` ➔ `In Progress` ➔ `Resolved`), and admin remark audit threads.
4. **Digital Gate Pass**: Exit requests, curfew tracking, parent consent verification, and verifiable pass tokens (`GP-XXXX`).
5. **Mess & Dietary Operations**: 7-day weekly menu management with student ratings and feedback analytics.
6. **Community & Lost-and-Found**: Real-time broadcasts, community chat, and photo-verified item claim workflow.

---

## 🚀 One-Click Deployments

### 🌐 1. Deploy Frontend to Vercel
You can deploy `Hostel-Frontend` directly on [Vercel](https://vercel.com):

1. Go to your **Vercel Dashboard** and click **"Add New Project"**.
2. Import the repository: `https://github.com/RohithSV2/Hostel-App`.
3. Configure Project Settings:
   - **Root Directory**: `Hostel-Frontend`
   - **Framework Preset**: `Other`
   - **Build Command**: `npm run build` *(or `npx expo export -p web`)*
   - **Output Directory**: `dist`
4. Click **Deploy**. Vercel will build and serve your web application.

---

### ☁️ 2. Deploy Backend to Render
You can deploy `Hostel-Backend` directly on [Render](https://render.com):

1. Go to your **Render Dashboard** and click **"New +" ➔ "Web Service"**.
2. Connect your GitHub repository: `RohithSV2/Hostel-App`.
3. Configure Service:
   - **Name**: `hostelmate-backend`
   - **Root Directory**: `Hostel-Backend`
   - **Runtime**: `Node`
   - **Build Command**: `npm install`
   - **Start Command**: `node server.js`
   - **Environment Variables**:
     - `PORT`: `10000`
     - `NODE_ENV`: `production`
     - `JWT_SECRET`: *(your secret key)*
4. Click **Create Web Service**.
*(On the first launch, the backend automatically detects a fresh database and auto-seeds all rooms, menus, demo accounts, and passes).*

---

## 🔑 Demo Credentials

| Role | Email | Password | Assigned Room / Bed |
| :--- | :--- | :--- | :--- |
| **Chief Warden / Admin** | `admin@test.com` | `123456` | Admin Office |
| **Student Resident 1** | `student@test.com` | `123456` | Room 101 — Bed A |
| **Student Resident 2** | `rahul@test.com` | `123456` | Room 101 — Bed B |

---

## 💻 Local Development Setup

### Backend
```bash
cd Hostel-Backend
npm install
node server.js
```
Runs at `http://localhost:5000`.

### Frontend
```bash
cd Hostel-Frontend
npm install
npx expo start
```
Press `a` for Android Emulator, `w` for Web preview, or scan the QR code via Expo Go on iOS/Android.
