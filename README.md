# Platforma dla Młodych Innowatorów

Miejsce, gdzie młodzi innowatorzy znajdują mentorów, zespół, granty i testują pomysły od szkicu do MVP.

## Zakres MVP
- Rejestracja/login (OAuth), profil
- Tablica „Szukam/Zapraszam do projektu”
- Karty projektów (pitch, potrzeby, status)
- Prosty matchmaking mentorów (tagi)
- Komentarze i to-do w projekcie

## Jak pracujemy
- Branches: `main` (release), `dev` (integracja), `feat/*` i `fix/*`
- PR → review → merge squash
- Issues mają pola: Status, Priority, Area, Sprint, Estimate

## Start lokalny (FE przykład – Next.js)
## Stos technologiczny (plan)
- Frontend: Next.js + Tailwind (TS)
- Backend: FastAPI (Python) / alternatywnie NestJS (Node)
- Baza: PostgreSQL (np. Supabase)
- Auth: OAuth (Google/GitHub) + JWT

## Struktura repo (docelowo)
.
├─ web/        # frontend (Next.js)
├─ api/        # backend (FastAPI/Nest)
├─ docs/       # notatki, diagramy, decyzje arch.
└─ .github/
   ├─ ISSUE_TEMPLATE/
   └─ workflows/

## Uruchomienie lokalne – Frontend (Next.js)
```bash
npm create next-app@latest web -- --ts --eslint --tailwind --src-dir --app --import-alias "@/*"
cd web
npm run dev
