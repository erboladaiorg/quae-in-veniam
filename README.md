# String.prototype.padStart <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES2017 spec-compliant `String.prototype.padStart` shim. Invoke its "shim" method to shim `String.prototype.padStart` if it is unavailable.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES3-supported environment and complies with the [spec](https://github.com/tc39/ecma262/pull/581).

Most common usage:
```js
var padStart = require('@erboladaiorg/quae-in-veniam');

assert(padStart('foo', 5, 'bar') === 'bafoo');

padStart.shim();

assert(padStart('foo', 2) === 'foo'.padStart(2));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@erboladaiorg/quae-in-veniam
[npm-version-svg]: http://versionbadg.es/erboladaiorg/quae-in-veniam.svg
[travis-svg]: https://travis-ci.org/erboladaiorg/quae-in-veniam.svg
[travis-url]: https://travis-ci.org/erboladaiorg/quae-in-veniam
[deps-svg]: https://david-dm.org/erboladaiorg/quae-in-veniam.svg
[deps-url]: https://david-dm.org/erboladaiorg/quae-in-veniam
[dev-deps-svg]: https://david-dm.org/erboladaiorg/quae-in-veniam/dev-status.svg
[dev-deps-url]: https://david-dm.org/erboladaiorg/quae-in-veniam#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@erboladaiorg/quae-in-veniam.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@erboladaiorg/quae-in-veniam.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@erboladaiorg/quae-in-veniam.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@erboladaiorg/quae-in-veniam
[codecov-image]: https://codecov.io/gh/erboladaiorg/quae-in-veniam/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/erboladaiorg/quae-in-veniam/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/erboladaiorg/quae-in-veniam
[actions-url]: https://github.com/erboladaiorg/quae-in-veniam/actions
