# Prettier setup

My preferred [Prettier](https://prettier.io/) setup.

## Prettier version

This config is compatible with Prettier version 2.x.x. It will be reviewed if
and when there is a new major release.

## Approach

I've only specified options which differ from the default values. Updates to
default values are considered a breaking change, so this config will remain
valid until a new major release.

## Usage

Copy `.prettierrc` and `.prettierignore` into your project, then customise
`.prettierignore` if necessary.

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
