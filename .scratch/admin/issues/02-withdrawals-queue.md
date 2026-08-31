# Admin withdrawals queue

Type: task
Status: ready
Blocked by:

## Goal

Очередь заявок: `GET/PATCH /api/v1/admin/withdrawals` confirm/reject.

## Canon

См. `docs/04_payments.md` (пилот, ручное подтверждение),
`docs/api-contracts/endpoints.md`. Денежный экран — ручной review.

## Scope

- Список pending
- Действия approve/reject
- Не делать вид, что деньги ушли в банк

## Out of scope

- ISO 20022
- Массовый approve без подтверждения

## Done

- [ ] Статус обновляется с API
- [ ] Conflict уже обработанной заявки показан

## Comments
