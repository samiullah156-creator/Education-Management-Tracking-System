<!-- styled:v2 -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1d1726,50:167dfe,100:9533fa&height=180&section=header&text=Education%20Management%20%26%20Tracking%20System%20(EMTS)&fontSize=25&fontColor=ffffff&fontAlignY=36&desc=React%20%E2%80%A2%20Redux%20%E2%80%A2%20Node.js&descAlignY=58&descSize=16&animation=fadeIn" width="100%" alt="Education Management & Tracking System (EMTS)" />

**A full-stack MERN school management system for admins, teachers, students and parents, with attendance, fees, chat and AI-written student reports.**

<p>
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Redux%20Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white" alt="Redux" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
</p>

<p>
  <a href="#overview">Overview</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#features">Features</a> ·
  <a href="#tech-stack">Tech stack</a> ·
  <a href="#project-structure">Project structure</a> ·
  <a href="#getting-started">Getting started</a>
</p>

</div>

---

## Overview

Schools juggle attendance sheets, fee records and parent messages across paper and WhatsApp. EMTS puts them in one web app with a separate dashboard for every role, real-time chat and AI-generated performance reports for each student.

## Features

| Role | What they can do |
|:--|:--|
| 🛡️ **Admin** | Manage teachers, students and classes, track fees, message teachers |
| 👩‍🏫 **Teacher** | Mark attendance, record results, chat with admin and parents |
| 🎓 **Student** | See attendance, results and fee status |
| 👪 **Parent** | Monitor their child's attendance and progress, chat with teachers |

- Login and registration with Firebase Authentication
- Attendance management and fee tracking
- Real-time chat and notifications (Firebase Firestore)
- AI-based student performance reports
- Role-based dashboards and protected routes

## How it works

```mermaid
flowchart LR
    U([Admin / Teacher /<br/>Student / Parent]) --> F[React + Redux<br/>frontend]
    F --> A[Firebase Auth]
    F --> B[Express API]
    B --> M[(MongoDB)]
    F --> C[(Firestore<br/>chat + notifications)]
    B --> AI([AI student<br/>reports])

    classDef box fill:#1d1726,stroke:#167dfe,color:#e5e7eb
    classDef ends fill:#2e1065,stroke:#9533fa,color:#ffffff
    class F,A,B box
    class U,M,C,AI ends
```

## Tech stack

| Layer | Tools |
|:--|:--|
| Frontend | React, Redux Toolkit, React Router, Bootstrap, Tailwind CSS |
| Backend | Node.js, Express, Mongoose |
| Data | MongoDB, Firebase Firestore |
| Auth | Firebase Authentication |

## Project structure

```
├── backend/     # Express API: controllers, models, routes, index.js
└── frontend/    # React app: pages, components, redux, firebase.js
```

## Getting started

```bash
cd backend && npm install
cd ../frontend && npm install
```

Create `backend/.env`:

```env
MONGO_URL=your_mongodb_connection_string
FIREBASE_API_KEY=your_firebase_api_key
PORT=5000
```

```bash
cd backend && npm start     # http://localhost:5000
cd frontend && npm start    # http://localhost:3000
```

## License

MIT

---

<div align="center">

**Built by [Ch Muhammad Samiullah](https://github.com/samiullah156-creator)** · AI Automation Engineer and Full-Stack Developer at [Lexvaxa](https://lexvaxa.com)

<a href="https://github.com/samiullah156-creator"><img src="https://img.shields.io/badge/More%20projects-181717?style=for-the-badge&logo=github&logoColor=white" alt="More projects" /></a>
<a href="https://lexvaxa.com/contact"><img src="https://img.shields.io/badge/Work%20with%20me-167dfe?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Work with me" /></a>
<a href="https://www.linkedin.com/in/sami-lexvaxa/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

<sub>⭐ Star this repo if you found it useful</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:9533fa,50:167dfe,100:1d1726&height=110&section=footer" width="100%" alt="" />
