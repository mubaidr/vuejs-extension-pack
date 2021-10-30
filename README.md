# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Recommended ESlint setup

### ESLint with vue and typescipt

#### Install following packages

```bash
npm install --save-dev eslint vue-eslint-parser @typescript-eslint/parser @typescript-eslint/eslint-plugin eslint-plugin-vue eslint-plugin-prettier eslint-config-prettier
```

#### Create/update eslint config

```ts
// enable vue in eslint

module.exports = {
  parser: "vue-eslint-parser",
  parserOptions: {
    parser: "@typescript-eslint/parser",
  },
  plugins: ["vue", "@typescript-eslint"],
  extends: [
    "eslint:recommended",
    "plugin:@typescript-eslint/eslint-recommended",
    "plugin:@typescript-eslint/recommended",
    "plugin:vue/essential",
    "plugin:prettier/recommended",
  ],
};
```

### ESLint with vue and javascript

#### Install following packages

```bash
npm install --save-dev eslint vue-eslint-parser babel-eslint eslint-plugin-vue eslint-plugin-prettier eslint-config-prettier
```

#### Create/update eslint config

```js
// enable vue in eslint

module.exports = {
  parser: "vue-eslint-parser",
  parserOptions: {
    parser: "babel-eslint",
  },
  plugins: ["vue"],
  extends: [
    "eslint:recommended",
    "plugin:vue/essential",
    "plugin:prettier/recommended",
  ],
};
```

## Extensions Included in this pack

- [Vue Language Features (Volar)](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar) - Language support for Vue 3
- [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.vscode-typescript-vue-plugin) - Vue Plugin for TypeScript server
- [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) -
  Vue tooling for VSCode
- [Vue VSCode Snippets](https://marketplace.visualstudio.com/items?itemName=sdras.vue-vscode-snippets) - Snippets that will supercharge your Vue workflow
- [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) - Code snippets for JavaScript in ES6 syntax
- [formulahendry.auto-complete-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-complete-tag) -
  Extension Packs to add close tag and rename paired tag automatically for HTML/XML
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) -
  Integrates ESLint into VS Code.
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) -
  VS Code plugin for prettier/prettier
- [Formatting toggle](https://marketplace.visualstudio.com/items?itemName=tombonnike.vscode-status-bar-format-toggle) - A VS Code extension that allows you to toggle the formatter on and off with a simple click
- [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) - npm support for VS Code
- [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - Visual Studio Code plugin that autocompletes npm modules in import statements
- [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode) - AI-assisted development

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
