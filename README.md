# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Note

**Please read the [Recommended Settings](#Recommended-Settings) section to enable all features.**

## Recommended-Settings

### Setup VS Code

Enable FormatOnSave & Eslint for `.vue` files:

```js
"editor.formatOnSave": true,
"eslint.validate": [
  "javascript",
  "javascriptreact",
  "vue"
]
```

### Setup ESLint

Install following packages:

```sh
npm install --save-dev eslint-plugin-vue
npm install --save-dev eslint-config-prettier
```

Create/update eslint config file (`.eslintrc.js` or `.eslintrc.json`) in your project folder:

```js
// Sample `.eslintrc.js`

module.exports = {
  plugins: ['vue'], // enable vue plugin
  extends: ['plugin:vue/essential', 'prettier'], // activate vue related rules
}
```

## Extensions Included in this pack

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
* [Formatting toggle](https://marketplace.visualstudio.com/items?itemName=tombonnike.vscode-status-bar-format-toggle) - A VS Code extension that allows you to toggle the formatter on and off with a simple click
* [VS Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) - Adds real-time collaborative editing and debugging into VS Code.

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
