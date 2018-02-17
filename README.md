# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Note

Please read the [recommended settings](#Recommended-Settings) sections for best experience.

## Extensions Included

* [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) -
  Vue tooling for VSCode
* [vue-peek](https://marketplace.visualstudio.com/items?itemName=dariofuzinato.vue-peek) -
  Allows peek and goto definition for Vue single-file components
* [auto-rename-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) -
  Auto rename paired HTML/XML tag
* [auto-close-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) -
  Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime
  Text
* [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) -
  npm support for VS Code
* [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) -
  Code snippets for JavaScript in ES6 syntax
* [NPM IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) -
  Visual Studio Code plugin that autocompletes npm modules in import statements
* [Path IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) -
  Visual Studio Code plugin that autocompletes filenames
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) -
  Integrates ESLint into VS Code.
* [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) -
  VS Code plugin for prettier/prettier

## Recommended Settings

### VS Code

Update VS Code settings to enable `validate` and `autofix` for `vue` language:

```json
"prettier.eslintIntegration": true,
"eslint.autoFixOnSave": true,
"eslint.validate": [
  {
    "autoFix": true,
    "language": "javascript"
  },
  {
    "autoFix": true,
    "language": "vue"
  }
]
```

### ESLint

Install following packages:

```js
npm install --save-dev eslint-config-prettier
npm install --save-dev eslint-plugin-vue
```

Update eslint config (`.eslintrc.js` or `.eslintrc.json`):

```json
"plugins": ["vue"],
"extends": ["plugin:vue/recommended", "prettier"]
```

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
