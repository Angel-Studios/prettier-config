# `@Angel-Studios/prettier-config`

> Angel Studios [Prettier](https://prettier.io) config.

## Usage

**Install**:

```bash
$ npm i --saveDev @angel-studios/prettier-config
```
or
```bash
$ yarn add --dev @angel-studios/prettier-config
```

**Edit `package.json`**:

```jsonc
{
  // ...
  "devDependencies" {
    // ...
    "prettier": "^2.5.1",
  },
  "prettier": "@angel-studios/prettier-config"
}
```

### Configuring with eslint
```bash
$ npm i --saveDev eslint-config-prettier
```
or
```bash
$ yarn add --dev eslint-config-prettier
```

**Edit `eslintrc.js`**:

```jsonc
{
    // ...
    extends: [
        // ...
        'prettier'
    ]
}
```
