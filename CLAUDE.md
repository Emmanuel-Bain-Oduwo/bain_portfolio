# Project Rules for Claude

## Git Authorship — CRITICAL
- NEVER include Claude as git author, co-author, or any reference to Claude/Anthropic in commits, commit messages, PR titles, PR bodies, code comments, or any files pushed to this repository.
- All commits must be authored solely as: Emmanuel Bain Oduwo <bainemmanuel86@gmail.com>
- Always run before committing: `git config user.name "Emmanuel Bain Oduwo" && git config user.email "bainemmanuel86@gmail.com"`

## Google Search Console / Meta Tags
- Hardcode verification meta tags directly in the JSX `<head>` element in `layout.tsx` — do NOT use Next.js metadata `verification` field. Google cannot reliably find it via the metadata API abstraction.
- Working example:
  ```tsx
  <head>
    <meta name="google-site-verification" content="MOpMpC7zEDjlw_o2EEfwIY4imHUidnvvxFnztECcpTo" />
    ...
  </head>
  ```

## Site
- Live at: https://www.bainiac.me
- Frontend: Vercel (Next.js 14, TypeScript, Tailwind CSS, Framer Motion)
- Backend: Railway (FastAPI, SQLAlchemy, PostgreSQL)
- Contact email: emmanuelbain@kemirix.com
