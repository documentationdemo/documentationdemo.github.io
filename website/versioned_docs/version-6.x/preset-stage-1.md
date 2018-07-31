---
id: version-6.x-babel-preset-stage-1
title: babel-preset-stage-1
sidebar_label: stage-1
original_id: babel-preset-stage-1
---

The gist of Stage 1 is:

> **Stage 1**: proposal
>
> **What is it?** A formal proposal for the feature.
>
> **What’s required?** A so-called champion must be identified who is responsible for the proposal. Either the champion or a co-champion must be a member of TC39 (source). The problem solved by the proposal must be described in prose. The solution must be described via examples, an API and a discussion of semantics and algorithms. Lastly, potential obstacles for the proposal must be identified, such as interactions with other features and implementation challenges. Implementation-wise, polyfills and demos are needed.
>
> **What’s next?** By accepting a proposal for stage 1, TC39 declares its willingness to examine, discuss and contribute to the proposal. Going forward, major changes to the proposal are expected

This preset includes the following plugins:

- [transform-class-constructor-call](https://babeljs.io/docs/en/babel-plugin-transform-class-constructor-call) (Deprecated)
- [transform-export-extensions](https://babeljs.io/docs/en/babel-plugin-transform-export-extensions)

And all plugins from presets:

- [preset-stage-2](https://babeljs.io/docs/en/babel-preset-stage-2)
- [preset-stage-3](https://babeljs.io/docs/en/babel-preset-stage-3)

> You can check the src/index.js to be sure the plugins used.

## Install

```sh
npm install --save-dev babel-preset-stage-1
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "presets": ["stage-1"]
}
```

### Via CLI

```sh
babel script.js --presets stage-1
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  presets: ["stage-1"]
});
```

## References

- Chapter "[The TC39 process for ECMAScript features](http://exploringjs.com/es2016-es2017/ch_tc39-process.html)" in "Exploring ES2016 and ES2017" by Axel Rauschmayer

