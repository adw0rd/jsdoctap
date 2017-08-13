# jsdoctap

Doctests using JSDoc examples and node-tap.

Based on the hard work of [@yamadapc](https://github.com/yamadapc) and [this
project](https://github.com/yamadapc/jsdoctest).

* [Examples](./examples)
* [Roadmap](./ROADMAP.md)
* [Changes](./CHANGELOG.md)

![screenshot](http://zacanger.com/jsdoctap.gif)

--------

## Installation

`npm i -D jsdoctap`

## Usage

`jsdoctap some-file.js`

I recommend adding it to your npm scripts. Example:

```json
{
  "scripts": {
    "test": "jsdoctap src/*.js"
  }
}
```

### Format

Tests must be valid JavaScript under an `@example` in a valid JSDoc comment.
The return value to be tested against must come after a line comment with an
arrow (Clojure REPL style):

```javascript
/**
 * Identity
 * @example
 * id(1) // => 1
 */
```

Line breaks between the call and the comment are fine:

```javascript
/**
 * Identity
 * @example
 *   id(1)
 *   // => 1
 */

```

## License

[MIT](./LICENSE.md)
