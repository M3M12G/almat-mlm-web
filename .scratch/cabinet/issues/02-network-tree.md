# Network tree in cabinet

Type: task
Status: ready
Blocked by:

## Goal

Визуализировать `GET /api/v1/network/tree` в ЛК. Здесь можно добавить
`@xyflow/react` (AGENTS.md: не раньше этого экрана).

## Canon

См. `docs/TECH_SPEC.md` §4.1 (xyflow MIT core), `docs/api-contracts/endpoints.md`.

## Scope

- Depth как отдаёт API (не просить всю компанию)
- Read-only; без drag-reparent
- Пустое дерево — empty state, не ошибка

## Out of scope

- Редактирование спонсора
- Stats / объёмы
- Recharts

## Done

- [ ] Первая линия видна
- [ ] Нет второго UI-kit, только xyflow + shadcn

## Comments
