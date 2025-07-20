# 📦 Week 7 DevOps Deployment Assignment

This is a full-stack MERN application demonstrating deployment using **Render** and automation with **GitHub Actions** for **CI/CD**.

---

## 🌍 Live URLs

- **Frontend**: [https://week-7-devops-deployment-assignment-nz2z.onrender.com](https://week-7-devops-deployment-assignment-nz2z.onrender.com)  
- **Backend**: [https://week-7-devops-deployment-assignment-0pzn.onrender.com](https://week-7-devops-deployment-assignment-0pzn.onrender.com)

---

## 📁 Folder Structure

```
├── client       # React frontend
├── server       # Express backend
├── .github
│   └── workflows
│       ├── frontend-ci.yml
│       ├── backend-ci.yml
│       ├── frontend-cd.yml
│       └── backend-cd.yml
```

---

## 🚀 Deployment Platform

We used **Render.com** to host both the frontend and backend:

- Frontend deployed from `client/`
- Backend deployed from `server/`

---

## ⚙️ GitHub Actions Workflows

### ✅ CI (Continuous Integration)

- **frontend-ci.yml**: Runs test commands or basic checks on every frontend push.
- **backend-ci.yml**: Runs basic checks on backend code.

### 🚀 CD (Continuous Deployment)

- **frontend-cd.yml**: Automatically deploys frontend to Render on changes to `client/`.
- **backend-cd.yml**: Automatically deploys backend to Render on changes to `server/`.

Each uses a `curl` request to trigger deployment using the Render deploy hooks.

---

## 🔍 Monitoring and Maintenance

### Monitoring Tools Used

- **Render logs** for checking build and runtime issues
- **UptimeRobot** to monitor frontend and backend URLs and send alerts if they're down

### Maintenance Strategy

- **Weekly**: Check Render logs and monitor uptime
- **Monthly**:
  - Run `npm update` in `client/` and `server/`
  - Review GitHub workflows and test pipelines
- **Database**: MongoDB Atlas handles automated backups

---

## 📦 Technologies Used

- **Frontend**: React (Vite or CRA)
- **Backend**: Express.js, Node.js
- **Database**: MongoDB (via Atlas)
- **CI/CD**: GitHub Actions
- **Hosting**: Render

---

## 👩‍💻 How to Run Locally

```bash
# Frontend
cd client
npm install
npm run dev

# Backend
cd server
npm install
npm run dev
```

---
