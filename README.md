# eOffice Correspondence

Developed during a project-based internship at a regional government institution in Indonesia. This MEVN application brings letter intake, attachments, disposition, archiving, user management, and staff chat into one interface.

## What it does

- Creates and updates letter records with sender, number, date, subject, status, and attachments.
- Records recipients, disposition instructions, notes, and follow-up status.
- Moves letters into an archive with a reference to the original record.
- Provides user accounts and an internal chat using Socket.IO.
- Supports placing a signature or initial on document attachments in the interface.

## Stack

MongoDB, Express, Node.js, Vue 3, Vue Router, Vuex, Socket.IO, Multer, and PDF editing libraries.

## Run locally

Copy `.env.example` to an untracked `.env` file, configure a local MongoDB connection, and set a fresh `JWT_SECRET`. Then:

```bash
npm install
cd frontend && npm install && cd ..
npm run dev
```

The frontend expects the development API at `http://localhost:3000` and runs through Vue CLI at `http://localhost:8080`.

## Project structure

- `routes/` — correspondence, archive, and user API routes.
- `model/` — MongoDB models for letters, archives, users, and chat.
- `frontend/src/components/` — letter management, archive, signature, and user interfaces.
- `frontend/src/services/` — API clients and frontend state.

## Portfolio note

This is a clean portfolio snapshot, not a hosted public demo. User-uploaded documents and signatures are intentionally excluded. The `uploads/` directory is created locally when needed and ignored by Git. This repository starts with a new history; it does not carry the original development uploads. The MIT license and attribution for the original MEVN authentication scaffold are retained.
