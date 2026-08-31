# Register page

Type: task
Status: ready
Blocked by:

## Goal

Регистрация с `referral_code` на `(public)/register` → `POST /api/v1/auth/register`.

## Canon

См. `docs/api-contracts/endpoints.md`, `docs/TECH_SPEC.md` §4.

## Scope

- Поля: email, password, referral_code (query `?ref=` предзаполняет)
- Cookie session после успеха, редирект cabinet
- Валидация неизвестного кода с API

## Out of scope

- SMS verify
- Выбор спонсора вручную кроме кода

## Done

- [ ] `?ref=` попадает в форму
- [ ] Успех создаёт сессию без второго логина

## Comments
