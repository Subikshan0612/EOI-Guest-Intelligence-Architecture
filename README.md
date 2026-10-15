# EOI Guest Intelligence — Architecture

This repository contains the interactive master architecture of the EOI Guest Intelligence platform.

## Purpose

A standalone, shareable viewer for the final EOI Guest Intelligence master architecture. It is deployed as a static page so stakeholders can open the architecture from a single URL, without access to the application codebase.

## Architecture overview

The root page (`index.html`) is the interactive master architecture diagram of the EOI Guest Intelligence platform. It is a plain static site: no framework, no build step, no server-side code.

## Run locally

Open `index.html` directly in a browser, or serve the folder:

```bash
npx serve .
```

or

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy to Vercel

1. Push this repository to GitHub.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Framework preset: **Other**. Leave build command and output directory empty (the repo root is served as-is).
4. Deploy. The root URL opens the master architecture directly.

Alternatively, with the Vercel CLI: `vercel --prod` from this folder.

## Source project reference

The architecture was produced from the EOI Guest Intelligence project (source file: `03-eoi-master-architecture.html`, served here as `index.html`). This repository contains no application code, secrets, or credentials.
