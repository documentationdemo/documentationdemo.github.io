---
id: version-6.x-babel-preset-stage-0
title: babel-preset-stage-0
sidebar_label: stage-0
original_id: babel-preset-stage-0
---

The gist of Stage 0 is:

> **Stage 0**: strawman
>
> **What is it?** A free-form way of submitting ideas for evolving ECMAScript. Submissions must come either from a TC39 member or a non-member who [has registered as a TC39 contributor](http://www.ecma-international.org/memento/contribute_TC39_Royalty_Free_Task_Group.php).
>
> **What’s required?** The document must be reviewed at a TC39 meeting (source) and is then added to [the page with stage 0 proposals](https://github.com/tc39/proposals/blob/master/stage-0-proposals.md).

This preset includes the following plugins:

- [transform-do-expressions](https://babeljs.io/docs/en/babel-plugin-transform-do-expressions)
- [transform-function-bind](https://babeljs.io/docs/en/babel-plugin-transform-function-bind)

And all plugins from presets:

- [preset-stage-1](https://babeljs.io/docs/en/babel-preset-stage-1)
- [preset-stage-2](https://babeljs.io/docs/en/babel-preset-stage-2)
- [preset-stage-3](https://babeljs.io/docs/en/babel-preset-stage-3)

> You can check the src/index.js to be sure the plugins used.

## Install

```sh
npm install --save-dev babel-preset-stage-0
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "presets": ["stage-0"]
}
```

### Via CLI

```sh
babel script.js --presets stage-0
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  presets: ["stage-0"]
});
```

## References

- Chapter "[The TC39 process for ECMAScript features](http://exploringjs.com/es2016-es2017/ch_tc39-process.html)" in "Exploring ES2016 and ES2017" by Axel Rauschmayer

