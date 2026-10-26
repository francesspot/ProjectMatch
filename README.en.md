🇵🇱 [Polski](README.md) | 🇬🇧 **English**

# 🤝 ProjectMatch

![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

> 🎓 Open-source project for the **KN Solvro** student research group (Wrocław University of Science and Technology), developed in collaboration with [Jan Wojtysiak](https://github.com/JanWojtysiak). Formerly called **Wakajki**.

A web app that helps participants of the KN Solvro Summer Challenge find a team for a shared project. Users sign in with Discord, create projects and join other people's projects.

> The project is in alpha.

## ✨ Features

- Sign-in with **Discord OAuth**
- Creating projects with a name, description and number of people needed
- **Open** projects (join instantly) and **closed** projects (join request that the owner accepts or rejects)
- Editing and deleting your own projects, leaving projects you joined
- Automatic refreshing of the project list

## 🙋 My contribution

- **Backend:** CRUD endpoints for projects, DTOs and API documentation in **Swagger**
- **Frontend:** the first version of the UI in React + Tailwind
- **Discord login** (Passport strategy, OAuth flow on both backend and frontend)
- Database schema changes and UI/UX improvements
- Automatic data refreshing and fixes to joining and leaving projects

## 🛠️ Tech

| Part | Technologies |
|---|---|
| Backend | NestJS, TypeScript, Prisma, PostgreSQL, Passport (Discord OAuth), Swagger |
| Frontend | React, Vite, TypeScript, Tailwind CSS |
| Infrastructure | Docker Compose |

## 🚀 Run it

Create a `.env` file from `.env.example` and fill in your Discord app credentials (`DISCORD_CLIENT_ID`, `DISCORD_CLIENT_SECRET`, `DISCORD_CALLBACK_URL`, by default `http://localhost:3000/auth/discord/callback`), then:

```bash
docker compose up --build
```

Frontend: <http://localhost:5173> · API: <http://localhost:3000> · API docs: <http://localhost:3000/api>

The interface is in Polish.
