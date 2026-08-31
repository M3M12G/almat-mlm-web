# Shop package list

Type: task
Status: ready
Blocked by:

## Goal

`(shop)/shop` рендерит пакеты из `GET /api/v1/catalog/packages`.

## Canon

См. `docs/TECH_SPEC.md` §4.2, `docs/api-contracts/endpoints.md`.

## Scope

- Карточки START / BUSINESS / PREMIUM (цена из API, не хардкод)
- CTA «купить» может вести на checkout (тикет 02) или disabled, пока 02 blocked
- Auth: если API `[Authorize]`, редирект на login

## Out of scope

- Оплата
- Корзина multi-item

## Done

- [ ] Три пакета с серверными ценами
- [ ] Empty/error state

## Comments
