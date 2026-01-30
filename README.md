# learn-vue-3

Learning Vue 3 with hands-on.
This template should help get you started developing with Vue 3 in Vite.

**table of contents**

- [learn-vue-3](#learn-vue-3)
  - [Recommended IDE Setup](#recommended-ide-setup)
    - [Customize configuration](#customize-configuration)
    - [Type Support for `.vue` Imports in TS](#type-support-for-vue-imports-in-ts)
  - [Recommended Browser Setup](#recommended-browser-setup)
  - [Project Setup](#project-setup)
  - [Run localhost](#run-localhost)
    - [Run End-to-End Tests with Playwright](#run-end-to-end-tests-with-playwright)
  - [Build and Deploy](#build-and-deploy)
  - [Additional Docs](#additional-docs)

## Recommended IDE Setup

- IDE - [VSCode](https://code.visualstudio.com/)
- Extensions
  - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur)
  - Markdown

### Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

### Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Project Setup

- Clone the repo
- Install nvm [node version manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)
- Install node - `scripts/localhost.sh install` or `nvm use; npm install;`

## Run localhost

1. sync latest changes - `scripts/localhost.sh git`
2. Compile and Hot-Reload for Development - `npm run dev`
3. Lint with [ESLint](https://eslint.org/) - `npm run lint` and `npm run format`
4. Run Unit Tests with [Vitest](https://vitest.dev/) - `npm run test:unit`

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
```

## Build and Deploy

1. Type-Check, Compile and Minify for Production - `npm run build`
2. Deploy to gh-pages - `npm run deploy`

## Additional Docs

- [nvm](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)
- [vue 3](https://vuejs.org/guide/introduction)
- [node js](https://nodejs.org/en/learn/getting-started/introduction-to-nodejs)
- [gh pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
- [Create New and Setup](./docs/README.md)
