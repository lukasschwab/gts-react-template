# gts-react-template

A template repo for writing a React app in [Google Typescript Style](https://github.com/google/gts). Essentially `create-react-app` with some additional wrangling.

## Usage

1. Hit <kbd>Use this template</kbd> to create a new project repository.
2. Rename the app; use `ag gts-react-template`.
3. Check on the `typescript`, `gts`, `eslint` versions pinned in [package.json](./package.json); update them as appropriate.

To justupdate all dependencies to their latest versions:

```console
$ npx npm-check-updates -u
$ npm install
```

## Notes

Initialized a React app with GTS with the following steps (following [these instructions](https://ntsd.github.io/typescript-code-quality-with-gts/)).

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