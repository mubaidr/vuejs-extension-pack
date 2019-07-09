# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Note

**Please read & follow the [Recommended Settings](#Recommended-Settings) section to enable all features.**

## Recommended-Settings

### Setup VS Code

Enable FormatOnSave & Eslint for `.vue` files in VS Code settings:

```js
// enable vue language support

"eslint.options": {
  "extensions": [".js", ".vue"]
},
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

### Setup ESLint

- Install following packages:

```bash
npm install --save-dev eslint prettier babel-eslint eslint-plugin-vue eslint-plugin-prettier eslint-config-prettier vue-eslint-parser
```

- Create/update eslint config file (`.eslintrc.js` or `.eslintrc.json`) in your project folder:

```js
// enable vue in eslint

module.exports = {
  parser: 'vue-eslint-parser',
  parserOptions: {
    parser: 'babel-eslint'
  },
  plugins: ['vue'],
  extends: [
    'eslint:recommended',
    'plugin:vue/recommended',
    'prettier',
    'prettier/vue'
  ]
};
```

## Extensions Included in this pack

- [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) -
  Vue tooling for VSCode
- [vue-peek](https://marketplace.visualstudio.com/items?itemName=dariofuzinato.vue-peek) -
  Allows peek and goto definition for Vue single-file components
- [auto-rename-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) -
  Auto rename paired HTML/XML tag
- [auto-close-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) -
  Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime
  Text
- [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) -
  npm support for VS Code
- [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) -
  Code snippets for JavaScript in ES6 syntax
- [NPM IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) -
  Visual Studio Code plugin that autocompletes npm modules in import statements
- [Path IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) -
  Visual Studio Code plugin that autocompletes filenames
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) -
  Integrates ESLint into VS Code.
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) -
  VS Code plugin for prettier/prettier
- [Formatting toggle](https://marketplace.visualstudio.com/items?itemName=tombonnike.vscode-status-bar-format-toggle) - A VS Code extension that allows you to toggle the formatter on and off with a simple click
- [VSCode Essentials Snippets](https://marketplace.visualstudio.com/items?itemName=robertoachar.vscode-essentials-snippets) - A collection of essentials snippets for Visual Studio Code.

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
