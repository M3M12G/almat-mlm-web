# Login page

Type: task
Status: ready
Blocked by:

## Goal

Рабочий логин на `src/app/(public)/login/page.tsx` против
`POST /api/v1/auth/login` (cookie).

## Canon

См. `docs/TECH_SPEC.md` §4, `docs/api-contracts/endpoints.md`, ADR-0002.
TanStack Query. Не класть JWT в localStorage.

## Scope

- Форма email/password, shadcn
- credentials include (cookie)
- Ошибка — ProblemDetails, не сырой текст
- Редирект в cabinet при успехе
- Depends: api `identity-auth/02` (можно верстать против контракта)

## Out of scope

- 2FA
- OAuth

## Done

- [ ] Успешный логин открывает `/cabinet`
- [ ] Невалидные данные показывают ошибку, не ломают layout

## Comments
