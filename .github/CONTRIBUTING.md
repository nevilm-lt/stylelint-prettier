# Contributing

Thanks for contributing!

## Installation

```sh
git clone https://github.com/BPScott/stylelint-prettier.git
cd stylelint-prettier
yarn install
```

## Running the tests

```sh
yarn run test
```

This is a [Stylelint](https://stylelint.io/) plugin. Documentation for the APIs that it uses can be found on Stylelint's [Writing Plugins](https://stylelint.io/developer-guide/plugins/) page.

Linting is ran as part of `yarn run test`. The build will fail if there are any linting errors. You can run `yarn run lint --fix` to fix some linting errors (including formatting to match prettier's expectations). To run the tests without linting run `yarn run jest`.

This plugin is used to lint itself. The style is checked when `npm test` is run, and the build will fail if there are any linting errors. You can use `npm run lint -- --fix` to fix some linting errors. To run the tests without running the linter, you can use `node_modules/.bin/mocha`.

## Publishing

```bash
node build/release.js
git push --follow-tags
npm publish
```
