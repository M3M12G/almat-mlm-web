# Shop checkout (money screen)

Type: task
Status: blocked
Blocked by: 01

## Goal

`POST /orders` + редирект/оплата FreedomPay. Денежный экран — ручной review
перед merge (`AGENTS.md`).

## Canon

См. `docs/04_payments.md`, `docs/api-contracts/endpoints.md`.

## Scope

- Создать заказ, показать статус `pending` → `paid` (polling или return URL)
- Не считать бонусы на клиенте
- Depends: api `catalog-orders/02`, `payments/01`

## Out of scope

- Mock-оплата как единственный prod path
- Редактор суммы клиентом

## Stop

Не merge без human review денежного UI.

## Done

- [ ] Пользователь проходит покупку пакета на staging/test merchant
- [ ] Повторная кнопка не создаёт хаос (disable / idempotency как решит API)

## Comments
