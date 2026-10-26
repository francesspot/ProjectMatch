🇵🇱 **Polski** | 🇬🇧 [English](README.en.md)

# 🤝 ProjectMatch

![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

> 🎓 Projekt open source dla koła naukowego **KN Solvro** (Politechnika Wrocławska), rozwijany we współpracy z [Jan Wojtysiak](https://github.com/JanWojtysiak). Wcześniej pod nazwą **Wakajki**.

Aplikacja webowa, która pomaga uczestnikom Wakacyjnego Wyzwania KN Solvro znaleźć zespół do wspólnego projektu. Użytkownicy logują się przez Discorda, zakładają projekty i dołączają do projektów innych osób.

> Projekt jest w wersji alpha.

## ✨ Funkcje

- Logowanie przez **Discord OAuth**
- Zakładanie projektów z nazwą, opisem i liczbą potrzebnych osób
- Projekty **otwarte** (dołączenie od razu) i **zamknięte** (prośba o dołączenie, którą właściciel akceptuje lub odrzuca)
- Edycja i usuwanie własnych projektów, wychodzenie z projektów, do których się dołączyło
- Automatyczne odświeżanie listy projektów

## 🙋 Mój wkład

- **Backend:** endpointy CRUD dla projektów, DTO i dokumentacja API w **Swaggerze**
- **Frontend:** pierwsza wersja interfejsu w React + Tailwind
- **Logowanie przez Discorda** (strategia Passport, przepływ OAuth po stronie backendu i frontendu)
- Zmiany w schemacie bazy i poprawki UI/UX
- Automatyczne odświeżanie danych oraz poprawki dołączania do projektów i wychodzenia z nich

## 🛠️ Technologie

| Część | Technologie |
|---|---|
| Backend | NestJS, TypeScript, Prisma, PostgreSQL, Passport (Discord OAuth), Swagger |
| Frontend | React, Vite, TypeScript, Tailwind CSS |
| Infrastruktura | Docker Compose |

## 🚀 Uruchomienie

Utwórz plik `.env` na podstawie `.env.example` i uzupełnij dane aplikacji Discord (`DISCORD_CLIENT_ID`, `DISCORD_CLIENT_SECRET`, `DISCORD_CALLBACK_URL`, domyślnie `http://localhost:3000/auth/discord/callback`), a potem:

```bash
docker compose up --build
```

Frontend: <http://localhost:5173> · API: <http://localhost:3000> · Dokumentacja API: <http://localhost:3000/api>
