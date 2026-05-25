# DesignTokens

test project

## Overview

- Repository: [alzkdpf/DesignTokens](https://github.com/alzkdpf/DesignTokens)
- Visibility: Public
- Last updated: 2022-11-22
- Main stack: CSS, Node.js

## Project Structure

```text
.github/workflows/create-tokens.yml
.gitignore
LICENSE
README.md
build.js
custom.css
fns.js
index.html
output/dark.css
output/dark.json
output/global.css
output/global.json
output/light.css
output/light.json
package-lock.json
package.json
postcss.config.js
styles.css
tailwind.config.js
tailwind.css
tokens/dark.json
tokens/global.json
tokens/light.json
tokens.json
```

## Getting Started

Install dependencies or prepare the project:

```bash
npm install
```

Run the common development command:

```bash
npm run dev
```

## Available Scripts

- `build-transform-global`: `npx token-transformer tokens.json tokens/global.json global`
- `build-transform-light`: `npx token-transformer tokens.json tokens/light.json global,light,theme global`
- `build-transform-dark`: `npx token-transformer tokens.json tokens/dark.json global,dark,theme global`
- `build-transform`: `npm run build-transform-global && npm run build-transform-light && npm run build-transform-dark`
- `build-sd`: `node build.js`
- `build-tw`: `postcss ./styles.css -o ./tailwind.css`
- `build`: `npm run build-transform && npm run build-sd && npm run build-tw`

## Notes

- This README was generated from the repository metadata and file structure.
- Update this document when setup steps, deployment targets, or project ownership changes.
