# safeplacefound-AI-THERAPIST
# Therapy Chat App

Simple full-stack web app for guided, text-based conversations about mood, stress, and day-to-day problems.

> **Note**  
> This project is for learning / experimentation.  
> It is **not** professional therapy or medical advice.

---

## Features

- Chat-style interface with conversational responses
- User accounts (sign up / log in)
- Conversation history per user
- Optional mood check-ins before / after a chat
- Basic admin / config for system behaviour (tone, length, etc.)
- 
## Wellness Tools

This app also includes a small set of optional tools that can be used on their own
or alongside chat sessions:

- Panic room for moments of acute stress
- Journaling for tracking thoughts and patterns
- Audio-based calming content
- Lightweight physical activity encouragement

---

## Stack

Adjust this to your actual stack:

**Frontend**

- React / Next.js
- TypeScript
- Tailwind CSS (or your UI library)

**Backend**

- Node.js + Express (or NestJS, Django, etc.)
- REST API
- LLM provider integration (e.g. OpenAI API) for generating replies

**Database**

- PostgreSQL / MySQL / MongoDB
- ORM: Prisma / TypeORM / Mongoose

---

## Project Structure

```text
root
 ├─ backend/      # API, auth, DB, LLM calls
 ├─ frontend/     # UI, routing, chat screens
 └─ README.md
