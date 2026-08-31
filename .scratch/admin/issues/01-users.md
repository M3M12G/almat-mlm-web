# Admin users list

Type: task
Status: ready
Blocked by:

## Goal

`(admin)/admin` (или `/admin/users`): таблица из `GET /api/v1/admin/users`.

## Canon

См. `docs/api-contracts/endpoints.md`, `docs/TECH_SPEC.md` §4.2.

## Scope

- Поиск + пагинация
- Не показывать IIN/password
- 403 → понятный empty/forbidden, не dump JSON
- Смена спонсора в UI — опционально позже; если есть форма, только через
  PATCH с ошибкой цикла с API

## Out of scope

- Редактор бонус-правил
- Impersonation

## Done

- [ ] Админ видит список
- [ ] Не-админ не видит данные

## Comments
