# Fumadocs + TinaCMS (visual editing demo)

A [Fumadocs](https://fumadocs.dev) docs site with live visual editing enabled by [tina.io](https://tina.io), built to show
off [**tinacms-fumadocs-pkg**](https://github.com/0xharkirat/tinacms-fumadocs-pkg).

Edit your docs in a visual editor and watch the real Fumadocs components update as you
type. The `.mdx` files on disk stay the source of truth.

## Edit locally

```bash
pnpm dev
```

Open **http://localhost:3000/admin**, pick a doc, and edit. Saves write straight to the
`.mdx` files.

## Edit in production (TinaCloud)

This site is connected to TinaCloud: [Read TinaCloud setup docs](https://tina.io/docs/tinacloud/overview).

Open **https://fumadocs-with-tinacms-v1.vercel.app//admin** on the live site and edit there. Every save
commits to the `main` branch of this repo.

To protect `main`, point saves at a branch and turn on the editorial workflow:
[TinaCloud editorial workflow](https://tina.io/docs/tinacloud/editorial-workflow).

## Built with

[tinacms-fumadocs-pkg](https://github.com/0xharkirat/tinacms-fumadocs-pkg) wires the
TinaCMS editing layer into Fumadocs. Production rendering stays 100% Fumadocs.
