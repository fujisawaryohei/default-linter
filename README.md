# default-linter
ぼくのかんがえたさいきょうのりんたーかんきょう

## How to use
### clone this repository and install node_modules
```
git clone git@github.com:fujisawaryohei/default-linter.git
```
- npm
```
npm install
```
- yarn
```
yarn install
```

### At Project root directory
```
mkdir .vscode
touch settings.json
```
copy `vscode/settings.json` at this direcotry and paste that code to `.vscode/settings.json` at project root directory

### Edit settings.json
you must edit value at `"eslint.options"`
```
{
  "editor.formatOnSave": true,
  "eslint.format.enable": true,
  "eslint.options": {
    "configFile": "this repository path you clone"
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```

### For Example 
```
{
  "editor.formatOnSave": true,
  "eslint.format.enable": true,
  "eslint.options": {
    "configFile": "/Users/fujisawaryohei/JSLinter/typescript/browser/.eslintrc.json"
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```
