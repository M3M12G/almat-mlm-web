# Public auth

См. `docs/TECH_SPEC.md` §4, `docs/api-contracts/endpoints.md` (Auth),
ADR-0002 / ADR-0004. Страницы-stubs: `src/app/(public)/login/page.tsx`,
`register/page.tsx`.

JWT в httpOnly cookie — не класть токен в localStorage.

## Issues

| # | File | Status |
|---|---|---|
| 01 | [login](issues/01-login.md) | ready |
| 02 | [register](issues/02-register.md) | ready |
