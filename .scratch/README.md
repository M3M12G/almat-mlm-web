# .scratch — frontend tickets

One feature per folder: `.scratch/<feature-slug>/spec.md`.

**Link, don't copy** canon from the `docs/` submodule:

```markdown
См. `docs/TECH_SPEC.md` §4.2 и `docs/api-contracts/endpoints.md`.
```

See `docs/agents/issue-tracker.md`.

## Features (pilot handoff)

| Folder | Status | Notes |
|---|---|---|
| [public-auth](public-auth/spec.md) | ready | login / register against `/auth/*` |
| [cabinet](cabinet/spec.md) | ready | `/me` shell; tree after network API |
| [shop](shop/spec.md) | partial | catalog ready; checkout = money review |
| [admin](admin/spec.md) | ready | users + withdrawals queue |

Status on issue files: `ready` \| `blocked` \| `claimed` \| `resolved`.
