* Babel support
* Formatting of multi-line examples in output is totally wrong
* Fix blocks that use helper functions. Failing example:
    ```javascript
    const id = (a) => a
    map(id, [ 1, 2, 3, 4 ]) // => [ 1, 2, 3, 4 ]
    ```
* Clean up comment-parser and getModuleName (in tap)
* Quickcheck-like features?
* Type it (Flow, probably)
* More tests and examples
