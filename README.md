# gts-react-template

A template repo for writing a React app in [Google Typescript Style](https://github.com/google/gts) with [ESLint](https://eslint.org/).

This is roughly equivalent to running `create-react-app` and adding `gts`. When in conflict, I've preferred `gts`-recommended settings to `create-react-app`'s defaults.

## Why?

Provide an opinionated React template, with the dev tool niceties that come with opinionation. Make Typescript feel like Go.

## Usage

1. Hit <kbd>Use this template</kbd> to create a new project repository.
2. Rename the app; use `ag gts-react-template`.
3. Check on the `typescript`, `gts`, `eslint` versions pinned in [package.json](./package.json); update them as appropriate.

To bulk-update all dependencies to their latest versions:

```console
$ npx npm-check-updates -u
$ npm install
```

## Notes

This template is based on another unpublished project, in which I initialized a React app with `gts` (loosely tracking [these instructions](https://ntsd.github.io/typescript-code-quality-with-gts/)):

```console
$ npx create-react-app --template=typescript YOUR-APP-NAME
$ cd YOUR-APP-NAME
$ npx gts init
$ npm install eslint-plugin-react --save-dev
$ npm install eslint-plugin-node@latest --save-dev
$ npm install eslint-plugin-prettier@latest --save-dev
$ npx gts check
$ npx gts fix
```