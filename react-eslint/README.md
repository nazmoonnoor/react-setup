# React ESLint setup

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Dev Dependencies:

### `npm i prettier eslint-config-prettier eslint-plugin-prettier -D`

## Create Linting Configuration file manually

Create a .eslintrc file in the project root and enter the below contents:
```
{
  "extends": ["react-app", "plugin:prettier/recommended"],
  "rules": {
    "prettier/prettier": [
      "error",
      {
        "endOfLine": "auto"
      }
    ]
  }
}

```

## VS Code Setup

## Plugins

Need to install the below plugins:
ESLint by Dirk Baeumer
Prettier - Code formatter by Prettier

## Settings

Follow the below settings for VS Code -

Create a new folder called ".vscode" inside the project root folder
Create a new file called "settings.json" inside that folder.
Paste the below json in the newly created settings.json file and save the file.

```
{
  // Theme
  "workbench.colorTheme": "Dracula",

  // config related to code formatting
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "javascript.validate.enable": false, //disable all built-in syntax checking
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true,
  // emmet
  "emmet.triggerExpansionOnTab": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "files.autoSave": "onFocusChange"
}

```
