# BluMint game partner docs

The source of the BluMint game partner docs, served at <https://docs.blumint.com> by [Mintlify](https://mintlify.com).

This directory is mirrored to the public repository `BluMintInc/partner-docs` on every release, and the mirror is overwritten each time, so an edit made in the mirror is lost. Edit the docs here instead.

## Preview the site

Run these from the root of the repository that holds this directory:

```sh
npm run partner-docs:spec
npm run partner-docs:dev
```

`partner-docs:spec` writes `openapi.json` from the API route docs and the decision tables in `snippets/generated/answers/` from the answers BluMint acts on, so never edit any of them by hand. The screenshots, videos and lock screens under `images/` are captures of the BluMint app, so replace one by capturing it again, never by editing it. `partner-docs:dev` serves the site at <http://localhost:3333>.

## Before you commit

```sh
npm run partner-docs:mint -- format
```

This puts every page in Mintlify's canonical form, which the Partner Docs check requires.
