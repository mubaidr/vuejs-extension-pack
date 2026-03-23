# Vue.js Extension Pack

This extension pack adds features and language support for Vue.js, Nuxt, and TypeScript development with modern tooling including Tailwind CSS support.

## Extensions Included in this pack

### Vue & Nuxt Core

- [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) - Language support for Vue 3
- [Nuxtr](https://marketplace.visualstudio.com/items?itemName=Nuxtr.nuxtr-vscode) - An extension for Nuxt offering commands and tools to make your experience more pleasant
- [Nuxt DX Tools](https://marketplace.visualstudio.com/items?itemName=alimozdemir.vscode-nuxt-dx-tools) - Tools for auto-locating and navigating to auto-imported components, functions, routes and more
- [MDC - Markdown Components](https://marketplace.visualstudio.com/items?itemName=Nuxt.mdc) - Syntax highlighting for MDC (Markdown Components) files for Nuxt Content

### Snippets & Productivity

- [Vue VSCode Snippets](https://marketplace.visualstudio.com/items?itemName=sdras.vue-vscode-snippets) - Snippets that will supercharge your Vue workflow

### Build & Testing

- [Vite](https://marketplace.visualstudio.com/items?itemName=antfu.vite) - VS Code for Vite
- [Vitest](https://marketplace.visualstudio.com/items?itemName=vitest.explorer) - Run and debug Vitest test cases

### Code Quality

- [Oxc](https://marketplace.visualstudio.com/items?itemName=oxc.oxc-vscode) - Oxlint and Oxfmt editor integration - ultra-fast linter and formatter for JavaScript/TypeScript
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - VS Code plugin for prettier/prettier
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens) - Improve highlighting of errors, warnings and other language diagnostics
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - Spelling checker for source code

### TypeScript

- [Pretty TypeScript Errors](https://marketplace.visualstudio.com/items?itemName=yoavbls.pretty-ts-errors) - Make TypeScript errors prettier and more human-readable

### Tailwind CSS

- [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) - Intelligent Tailwind CSS tooling for VS Code

### Developer Experience

- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=editorconfig.editorconfig) - EditorConfig Support for Visual Studio Code
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) - Improve your code commenting with alert, informational, TODOs, and more
- [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost) - Display import/require package size in the editor
- [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - Autocomplete npm modules in import statements

## Recommended Settings

For the best experience, consider adding these settings to your workspace:

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.oxc": "explicit"
  },
  "tailwindCSS.includeLanguages": {
    "vue": "html"
  }
}
```

## Credits

All credits goes to original authors of the above mentioned extensions.

Happy Coding!
