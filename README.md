# jvm-deob

This module complements [`kylestev/jvm.js`](https://github.com/kylestev/jvm.js) by
exposing transformation functions used to deobfuscate class files.

## Usage

```js
import { Jar } from 'jvm';
import { UnusedFieldTransform } from 'jvm-deob';

Jar.unpack('/path/to/your.jar')
  .then(UnusedFieldTransform)
  // Transforms will return the passed in Jar object allowing for
  // easy interoperability with Promises as shown above.

```
