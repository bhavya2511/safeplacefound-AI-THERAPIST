<img width="3783" height="1743" alt="image" src="https://github.com/user-attachments/assets/04737251-0496-464f-b7e4-1e040356167e" /># safeplacefound-AI-THERAPIST
# Therapy Chat App

Simple full-stack web app for guided, text-based conversations about mood, stress, and day-to-day problems.

DESKTOP VIEW:
<img width="3804" height="1563" alt="image" src="https://github.com/user-attachments/assets/0706b6f2-d0fb-4b5f-84e7-f9a1fb012c2f" />
<img width="3837" height="1737" alt="image" src="https://github.com/user-attachments/assets/e32b3bb6-818e-4f1c-a6b3-874da893494a" />
<img width="3783" height="1743" alt="image" src="https://github.com/user-attachments/assets/6941046e-11d4-4177-b227-ef854c753feb" />
<img width="3780" height="1749" alt="image" src="https://github.com/user-attachments/assets/b7b12f45-f5d4-4698-8ccb-c9f199cfec3f" />

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


<img width="498" height="894" alt="image" src="https://github.com/user-attachments/assets/33375615-10ef-468b-b5be-2d75aed0668f" />


Getting Started
1. Clone
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
2. Backend
cd backend
cp .env.example .env

Fill in values like:

PORT=4000
DATABASE_URL=postgres://user:pass@localhost:5432/dbname
OPENAI_API_KEY=your_key_here  # optional
JWT_SECRET=change_me

Install + migrate + run:

npm install
# e.g. for Prisma
npx prisma migrate dev
npm run dev
3. Frontend
cd ../frontend
cp .env.example .env

Example env:

VITE_API_URL=http://localhost:4000
# or NEXT_PUBLIC_API_URL / REACT_APP_API_URL

Install + run:

npm install
npm run dev

App will be available on http://localhost:3000 or your configured dev port.

Configuration

System behaviour (tone, length, context) can be configured in a prompt or config file, e.g.:

backend/src/llm/prompt.ts

Tweakable items:

tone (casual / formal)

response length

how much previous context is sent

Limitations

Responses are auto-generated and can be wrong or unhelpful.

Do not rely on this for emergencies or serious mental health situations.

For any real issues, talk to a licensed professional or local helpline.

License

MIT (or choose another license).

## Project Structure

```text
root
 ├─ backend/      # API, auth, DB, LLM calls
 ├─ frontend/     # UI, routing, chat screens
 └─ README.md
