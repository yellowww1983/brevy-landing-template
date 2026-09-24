## @brevy/ui

Pages in this project are built from `@brevy/ui`. Its documentation ships inside the package, one markdown file per foundation, component, block and screen.

- Start with `node_modules/@brevy/ui/dist/docs/index.md`. It lists every entry with one line each and the file that documents it.
- Open only the files for the parts the page needs.
- Before building a section that no block covers, read `node_modules/@brevy/ui/dist/docs/rules.md`.

Open these files by path. Search skips `node_modules`, so it will not find them on its own.

## This project

- It is one landing page. The page is `src/app/page.tsx`; build it there, and split sections into files under `src/app/` when it gets long.
- Start the dev server with `pnpm dev` before you change anything, so the person you are working with watches the page change as you build it.
- If `pnpm` is not found, run `corepack enable` first, then `pnpm install`.
- Never a raw value: `bg-secondary`, not a hex in a class; `p-6`, not `p-[24px]`. Every colour, size, radius and spacing comes from the tokens.
- Do not edit anything in `vendor/` or `node_modules/`. The package is Brevy's and is shared; compose out of what it ships.
