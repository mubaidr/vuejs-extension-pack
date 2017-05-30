# Vue.js Extension Pack

This extension pack adds features for Vue.js development! These are some of my favorite extensions to make Vue.js development easier and fun. [Setup Guide for ESLint](#Recomended-Settings)

## Extensions Included

* [vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - Enable .vue files format, linting, IntelliSense and more.
* [vuehelper](https://marketplace.visualstudio.com/items?itemName=oysun.vuehelper) - Code snippets for Vue,Vue-router and Vuex.
* [auto-rename-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime Text.
* [auto-close-tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) - Auto rename paired HTML/XML tag.
* [ES Lint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Integrates [ESLint](http://eslint.org/) into VS Code.
* [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script) - Run npm scripts from the command palatte and validate the installed modules defined in `package.json`.
* [JavaScript (ES6) Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets) - Adds code snippets for JavaScript development in ES6 syntax.
* [Search node_modules](https://marketplace.visualstudio.com/items?itemName=jasonnutter.search-node-modules) - Quickly search for node modules in your project.
* [NPM IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - Adds IntelliSense for npm modules in your code.
* [Path IntelliSense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - Autocompletes filenames in your code.

## Recomended Settings & ESLint Setup

### Vetur

``` json
"vetur.format.js.InsertSpaceBeforeFunctionParenthesis": true,
// Whether to have initial indent for <style> section
"vetur.format.styleInitialIndent": true,
// Whether to have initial indent for <script> section
"vetur.format.scriptInitialIndent": true
```

### How to get ESLint work with .vue files

#### ESLint packages required (recomend to add in package.json)

``` string
"eslint": "^3.19.0",
"eslint-friendly-formatter": "^2.0.7",
"eslint-loader": "^1.7.1",
"eslint-plugin-html": "^2.0.0",
"eslint-config-standard": "^6.2.1",
"eslint-plugin-promise": "^3.4.0",
"eslint-plugin-standard": "^2.0.1"
```

#### vscode user settings

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
// Run the linter on save (onSave) or on type (onType)
"eslint.run": "onSave",
"eslint.autoFixOnSave": true
```

#### .eslintrc.json (in root of the project folder)

``` json
{
  "env": {
    "browser": true,
    "commonjs": true,
    "es6": true,
    "node": true
  },
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "sourceType": "module"
  },
  // https://github.com/feross/standard/blob/master/RULES.md#javascript-standard-style
  "extends": "standard",
  // required to lint *.vue files
  "plugins": [
    "html"
  ],
  "rules": {
    "no-const-assign": "warn",
    "no-this-before-super": "warn",
    "no-undef": "warn",
    "no-unreachable": "warn",
    "no-unused-vars": "warn",
    "constructor-super": "warn",
    "valid-typeof": "warn"
  }
}

```

## Add your extension to this pack

Open a PR and I'd be happy to take a look.

## Credits

All credits goes to original authors of the above mentioned extensions.

**Happy Coding!**
