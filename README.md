# Prettier setup

My preferred [Prettier](https://prettier.io/) setup.

## Prettier version

This config is compatible with Prettier version 3.x.x. It will be reviewed if
and when there is a new major release.

## Approach

I've only specified options which differ from the default values. Updates to
default values are considered a breaking change, so this config will remain
valid until a new major release.

## Usage

Copy `prettier.config.js` into your project. Note that this file is written
using ESM. If you're using CommonJS, you'll need to update the default export to
use `module.exports = config;`.

Install the latest version of `prettier`:

```bash
npm install --save-dev prettier
```

Add the following scripts to your `package.json`:

```json
{
  "scripts": {
    "format": "prettier --list-different --write .",
    "format:check": "prettier --check ."
  }
}
```

## Ignoring files

From version 3, Prettier will automatically ignore anything in your `.gitignore`
file. If you want to ignore additional files, create a `.prettierignore` file at
the root of your project.
