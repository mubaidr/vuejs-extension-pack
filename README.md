# Vue.js Extension Pack

This extension pack adds features for Vue.js development.

## Extensions Included

* [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - Vue tooling for VSCode
* [vue-peek](https://marketplace.visualstudio.com/items?itemName=dariofuzinato.vue-peek) - Allows peek and goto definition for Vue single-file components
* [Vue 2 Snippets](https://marketplace.visualstudio.com/items?itemName=hollowtree.vue-snippets) - A Vue.js 2 Extension
* [auto-rename-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - Auto rename paired HTML/XML tag
* [auto-close-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) - Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime Text
* [ES Lint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Integrates ESLint into VS Code
* [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) - npm support for VS Code
* [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) - Code snippets for JavaScript in ES6 syntax
* [NPM IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - Visual Studio Code plugin that autocompletes npm modules in import statements
* [Path IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - Visual Studio Code plugin that autocompletes filenames

## ESLint installation

You have to install following pakcage either globally or locally (preffered) as dev dependencies.

``` json
  "eslint-config-standard": "^10.2.1",
  "eslint-friendly-formatter": "^3.0.0",
  "eslint-loader": "^1.9.0",
  "eslint-plugin-html": "^3.2.0",
  "eslint-plugin-import": "^2.7.0",
  "eslint-plugin-node": "^5.1.1",
  "eslint-plugin-promise": "^3.5.0",
  "eslint-plugin-standard": "^3.0.1",
  "eslint-plugin-vue": "beta",
  "eslint": "^4.4.1"
```

### Create .eslintrc.json in project root

Open command pallet and enter `ESlint` then select `Create .eslintrc.json` file and add following settings:

``` json
  ...,
  "extends": [
        "eslint:recommended",
        "plugin:vue/recommended"
  ],
  ...
```

### ESLint: Enable validate and autofix for `.vue` files

``` json
"eslint.enable": true,
"eslint.options": {
"extensions": [
  ...,
  ".vue",
  ...
  ]
},
"eslint.validate": [
  ...,
  {
    "language": "vue"
  },
  ...
]
```

## Add an extension to this pack

Open a PR and I'd be happy to take a look.

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
