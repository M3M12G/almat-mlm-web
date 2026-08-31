# Cabinet shell + /me

Type: task
Status: ready
Blocked by:

## Goal

`(cabinet)/cabinet` показывает профиль из `GET /api/v1/me` (ранг, рефкод,
баланс 0).

## Canon

См. `docs/TECH_SPEC.md` §4.2, `docs/api-contracts/endpoints.md`.

## Scope

- Guard: без cookie → `/login`
- TanStack Query для `/me`
- Не показывать IIN/password
- Taste: product surfaces (AGENTS.md)

## Out of scope

- Дерево (тикет 02)
- История бонусов (деньги — отдельный review)

## Done

- [ ] Авторизованный видит свои данные
- [ ] 401 уводит на login

## Comments
