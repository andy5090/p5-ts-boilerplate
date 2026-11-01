# p5-template

Starter for a [p5.js](https://p5js.org/) project using

- p5 in global mode
- [Vite](https://vite.dev/) - build tool
- [TypeScript](https://www.typescriptlang.org/) - language

## Requirements

- Node.js 22.12 or newer (use a maintained, patched release)
- Yarn Classic 1.22.22, available through Corepack

## Start a new project

1. Optional: On this repo's GitHub page, click "Use this template" to create your own repo.
2. Clone the repo locally and `cd` into its directory.
3. Run `corepack yarn install --frozen-lockfile`.

## Development

1. Run `corepack yarn dev`.
2. Open the local URL printed by Vite (normally `http://localhost:5173`).
3. Make edits to `src/main.ts`.

Keep development and preview servers local. Do not expose them to untrusted networks using `--host 0.0.0.0`; deploy the static build instead. Do not disable Vite's host or filesystem restrictions.

## Validation and production build

```sh
corepack yarn install --frozen-lockfile
corepack yarn build
corepack yarn audit
corepack yarn serve
```

`build` runs TypeScript checks and creates `dist/`. The preview command serves that build locally (normally `http://localhost:4173`). Verify that the particle animation renders in both development and preview. Texture assets are imported through Vite so they are included in production builds.

## Lockfiles

Yarn is the primary package manager. `bun.lock` is a text-format mirror generated from `yarn.lock`; the obsolete binary `bun.lockb` has been removed. Bun users can run `bun install --frozen-lockfile`, `bun run build`, and `bun audit`.

When changing dependencies, update and validate both lockfiles together. Do not keep an old binary Bun lockfile alongside the text lockfile.
