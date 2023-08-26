# postcss-less

A [PostCSS](https://github.com/postcss/postcss) syntax for parsing [LESS](https://lesscss.org/).

## Install

```shell
npm install @stylelint-less/postcss-less --save-dev
```

## Usage

```js
const postcss = require('postcss');
const postcssLess = require('postcss-less');

const source = `
@a: 1;
@b: 2;
@a: 3;
`;

postcss(plugins)
  .process(source, { syntax: postcssLess })
  .then((result) => {
    console.log(result.content);
  });
```

## Note

This is a fork of [postcss-less](https://github.com/shellscape/postcss-less).
