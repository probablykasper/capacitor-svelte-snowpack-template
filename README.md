# Svelte template

Features:

- **Svelte**
- **TypeScript**
- **Snowpack** for fast builds
  - **esbuild** enabled using `experiments.optimize` setting
- **Preprocessor support** through `svelte-preprocess`
  - Pug and Sass are installed by default
- **Hot module replacement**
- **Prettier**

Limitations:

- Source maps are supported for `.ts` and `.svelte` files, but not for the preprocessors used inside `.svelte` files
- Linting for code-quality rules is not supported. Would need to use ESLint with eslint-plugin-svelte3, but that plugin needs to work with svelte-preprocess ([issue](https://github.com/sveltejs/eslint-plugin-svelte3/issues/10))

## Recommended VSCode extensions

- `svelte.svelte-vscode` for Svelte
- `syler.sass-indented` for Sass
- `esbenp.prettier-vscode` for Prettier

## Setup

`src/main.ts` is built and bundled into `build/bundle/`.

To disable source maps, disable `buildOptions.sourceMaps` in `snowpack.config.js`.

## Commands

### `npm run start`

Starts dev server

### `npm run build`

Builds and bundles

### `npm run lint`

Lint the project
