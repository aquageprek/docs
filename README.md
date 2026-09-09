# Zaqua documentation

This repository contains the Mintlify documentation for Zaqua products, including
LucentUI and Sonata.

## Local preview

Install the current Mintlify CLI and start the development server from the repository
root:

```bash
npm install -g mint
mint dev
```

The preview is available at `http://localhost:3000` by default.

## Validation

Run these checks before publishing:

```bash
mint validate
mint broken-links --check-anchors
mint a11y
```

Keep every page referenced by `docs.json`, add descriptive alternative text to images,
and use absolute documentation paths such as `/lucentui/get-started` for internal links.

## Publishing

The production documentation is connected to this repository through the Mintlify
GitHub integration. Push reviewed changes to the configured deployment branch to publish
them.

## Content ownership

LucentUI implementation details should be verified against the current theme and Editor
source before changing the docs. Do not document planned features as available features.
