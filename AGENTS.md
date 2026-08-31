# mlm-web — Agent Instructions

Frontend application **mlm-web** (Next.js App Router + TypeScript strict + shadcn/ui +
TanStack Query).  
Repo / local folder: `almat-mlm-web` (имя репозитория не меняется).

**Canonical docs:** git submodule at `docs/` → repo `almat-mlm-docs`  
- Tech spec §4: `docs/TECH_SPEC.md`  
- Stack: `docs/01_stack.md` · ADR-0002 / ADR-0004: `docs/adr/`  
- Open questions (bonus/payments blocked): `docs/07_open_questions.md`

Update docs submodule after canon changes:

```bash
cd docs && git pull origin main && cd ..
git add docs && git commit -m "chore: update docs submodule ref"
```

## Не трогать без подтверждения человека

1. **Стек фронта** — не менять самовольно (ADR-0002, ADR-0004).
2. **Денежные экраны** — ручной review.
3. **Новый npm** вне allow-list — спросить.
4. Не ставить Zustand/Redux, платные UI-kit.

## Stack (fixed)

- Next.js (`output: 'standalone'`), React, TS **strict**
- shadcn/ui + Tailwind · TanStack Query · `@xyflow/react` / Recharts по мере экранов
- Surfaces: `public` · `cabinet` · `shop` · `admin` (`src/app/(…)`)

## UI foundation (locked)

One system: **shadcn/ui** (`base-nova`) + Tailwind v4. Tokens in `src/app/globals.css`.
Do not add a second UI kit (Fluent / Carbon / Material / Radix Themes / MUI).

- Type: IBM Plex Sans + IBM Plex Mono via `next/font` (Cyrillic; Geist has no Cyrillic)
- Accent: teal `oklch(… 175)` — not gold, not purple
- Radius: `0.625rem` everywhere
- Icons: `lucide-react` (already in repo — do not mix families)
- Taste dials: product surfaces `4 / 2 / 7`, public `5 / 3 / 3`
- Skill: `.cursor/skills/design-taste-frontend` (Leonxlnx/taste-skill v2)
- Do not add Motion / Zustand / `@xyflow/react` / Recharts until those screens exist

## Agent skills

### Issue tracker

`.scratch/<feature-slug>/` — specs **link** to `docs/…`, never copy.
See `docs/agents/issue-tracker.md`.

### Domain docs

`docs/adr/` via submodule (path unchanged). See `docs/agents/domain.md`.

---

<!-- BEGIN:nextjs-agent-rules -->

# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->
