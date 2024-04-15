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
  ...require('@mapbox/prettier-config-docs'),
  tabWidth: 4
};
```

## How to release

From the main branch:

1. Run `npm version {major|minor|patch}`. Example (and usually): `npm version minor`.
2. Push changes.
3. Run `mbx npm publish` to publish the package to npm.

Dependabot will automatically update `@mapbox/prettier-config-docs` (within 1 day) to all site repositories. If you need it sooner, you can install this package in the repository by following the [install steps](#install).
