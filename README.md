# eslint-config-snak
- support typescript
- base airbnb

# install
```shell
# eslint is not required.
npm i -D eslint-config-snak
touch ./eslintrc.js
```

**./eslintrc.js**
```js
module.exports = {
  extends: ['eslint-config-snak'],
};
```

**vscode config**
**./.vscode/settings.json**
```json
{
  // eslint config
  "eslint.autoFixOnSave": true,
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    { "language": "typescript", "autoFix": true },
    { "language": "typescriptreact", "autoFix": true }
  ]
}
```