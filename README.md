# Vue.js Extension Pack

This extension pack adds features for Vue.js development! These are some of my favorite extensions to make Vue.js development easier and fun.

## Extensions Included

* [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - Enable .vue files Syntax Highlight, Format, Scaffold, Emmet, IntelliSense, linting and more.
* [auto-rename-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - Automatically add HTML/XML close tag.
* [auto-close-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) - Auto rename paired HTML/XML tag.
* [ES Lint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Integrates ESLint into VS Code.
* [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) - Run npm scripts from the command palatte.
* [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) - Adds code snippets for JavaScript development in ES6 syntax.
* [Search node_modules](https://marketplace.visualstudio.com/items?itemName=jasonnutter.search-node-modules) - Quickly search for node modules in your project.
* [NPM IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - Adds IntelliSense for npm modules in your code.
* [Path IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - Autocompletes filenames in your code.

## ESLint installation

You have to install following pakcage either globally or locally (preffered) as dev dependencies.

``` json
"eslint": "^4.1.1",
"eslint-config-standard": "^10.2.1",
"eslint-friendly-formatter": "^3.0.0",
"eslint-loader": "^1.8.0",
"eslint-plugin-html": "^3.0.0",
"eslint-plugin-vue": "beta",
"eslint-plugin-import": "^2.6.1",
"eslint-plugin-node": "^5.1.0",
"eslint-plugin-promise": "^3.5.0",
"eslint-plugin-standard": "^3.0.1"
```

### Create .eslintrc.json in project root

Open command pallet and enter `ESlint` then select `Create .eslintrc.json` file and add following settings:

``` json
"extends": [
    "standard",
    "plugin:vue/recommended"
  ],
  "settings": {
    "html/html-extensions": [
      ".html"
    ],
    "html/report-bad-indent": "error"
  },
  // required to lint *.vue files
  "plugins": [
    "html"
  ]
```

### ESLint: Enable validate and autofix for `.vue` files

``` json
"eslint.enable": true,
"eslint.options": {
"extensions": [
  ".html",
  ".js",
  ".vue",
  ".jsx"
  ]
},
"eslint.validate": [{
  "language": "html",
  "autoFix": true
},
{
  "language": "vue",
  "autoFix": true
},
{
  "language": "javascript",
  "autoFix": true
},
{
  "language": "javascriptreact",
  "autoFix": true
}
],
"eslint.run": "onSave",
"eslint.autoFixOnSave": true
```

## Add your extension to this pack

Open a PR and I'd be happy to take a look.

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
