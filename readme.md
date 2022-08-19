# @esm2cjs/is-path-inside

This is a fork of https://github.com/sindresorhus/is-path-inside, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i is-path-inside@npm:@esm2cjs/is-path-inside
```

```jsonc
// package.json
"dependencies": {
    "is-path-inside": "npm:@esm2cjs/is-path-inside"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/is-path-inside
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/is-path-inside": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import isPathInside from "@esm2cjs/is-path-inside";

// Using CommonJS require()
const isPathInside = require("@esm2cjs/is-path-inside").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/is-path-inside).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/is-path-inside).
