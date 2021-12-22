# @Angel-Studios/prettier-config

> Angel Studios [Prettier](https://prettier.io) config.

## Caution

**If you are importing global styles, create one file that imports all of the others in the preferred order so that the order sorting plugin doesn't put them in the incorrect order.** 

## Usage

**Install**:

```bash
$ npm install -D prettier @angel-studios/prettier-config @trivago/prettier-plugin-sort-imports
```
or
```bash
$ yarn add --dev prettier @angel-studios/prettier-config @trivago/prettier-plugin-sort-imports
```

**Edit `package.json`**:

```jsonc
{
  // ...
  "prettier": "@angel-studios/prettier-config"
}
```

### Configuring with eslint
```bash
$ npm install -D eslint-config-prettier eslint-plugin-prettier
```
or
```bash
$ yarn add --dev eslint-config-prettier eslint-plugin-prettier
```

**Edit `eslintrc.js`**:

```jsonc
{
    // ...
    "extends": [
        // ...
        'prettier'
    ],
    "plugins": [
        // ...
        'prettier': 
    ],
    "rules": [
        // ...
        'prettier/prettier': 'error'
    ]
}
```

### Setup lint-stages / husky

Follow the steps below to setup lint-staged / husky and enable prettier running on every commit!

https://github.com/okonet/lint-staged

**Edit `package.json`**

```jsonc
{
  // ...
  "lint-staged": {
    "*.js": [
      "eslint --cache --fix"
    ],
    "*.{js,css,md}": "prettier --write"
  }
}
```
