# prettier-config-docs

[Prettier](https://prettier.io) configuration for docs.mapbox.com sites.

## Install

```bash
npm install --save-dev @mapbox/prettier-config-docs
```

Edit `package.json`:

```jsonc
{
 // ...
 "prettier": "@mapbox/prettier-config-docs"
}
```

_or_ to extend this configuration to overwrite some properties, create `.prettierrc.js`:

```js
module.exports = {
  ...require("@mapbox/prettier-config-docs"),
  "tabWidth": 4
};
```
