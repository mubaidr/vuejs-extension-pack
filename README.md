# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Note

Please read the [Recommended Settings](#Recommended-Settings) section to enable all features.

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
* [Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) - Beautify code in place for VS Code
* [Sorting HTML and Jade attributes](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-attrs-sorter) -
  Sorting of the tag attributes in the specified order

## Recommended-Settings

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
  },
  ...
]
```

Enable `Beautify` for HTML only (javascript/css is handled by `prettier`):

```json
"beautify.config": {
  "editorconfig": true,
  "indent_size": 2,
  "wrap_attributes": "force-aligned",
  "wrap_attributes_indent_size": 2,
  "wrap_line_length": 80
},
"beautify.language": {
  "html": [
    "htm",
    "html"
  ]
},
"vetur.format.defaultFormatter.html": "js-beautify-html",
"vetur.format.defaultFormatterOptions": {
  "js-beautify-html": {
    "editorconfig": true,
    "indent_size": 2,
    "wrap_attributes": "force-aligned",
    "wrap_attributes_indent_size": 2,
    "wrap_line_length": 80
  }
},
```

Enable eslint compatible and recommended settings for `Sorting HTML and Jade attributes`:

```json
"attrsSorter.order": [
    "is",
    "v-for",
    "v-if",
    "v-else-if",
    "v-else",
    "v-show",
    "v-cloak",
    "v-once",
    "v-pre",
    "id",
    "ref",
    "key",
    "slot",
    "v-model",
    "v-model.+",
    "v-bind",
    "v-bind.+",
    ":.+",
    "v-text",
    "v-text.+",
    "v-html",
    "v-html.+",
    "class",
    "v-on.+",
    "@.+",
    "name",
    "data-.+",
    "ng-.+",
    "src",
    "for",
    "type",
    "href",
    "values",
    "title",
    "alt",
    "role",
    "aria-.+",
    "$unknown$"
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
"extends": [/*airbnb or standard*/,"plugin:vue/recommended", "prettier"]
```

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
