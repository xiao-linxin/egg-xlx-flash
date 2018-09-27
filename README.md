# egg-xlx-flash

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/egg-xlx-flash.svg?style=flat-square
[npm-url]: https://npmjs.org/package/egg-xlx-flash
[travis-image]: https://img.shields.io/travis/eggjs/egg-xlx-flash.svg?style=flat-square
[travis-url]: https://travis-ci.org/eggjs/egg-xlx-flash
[codecov-image]: https://img.shields.io/codecov/c/github/eggjs/egg-xlx-flash.svg?style=flat-square
[codecov-url]: https://codecov.io/github/eggjs/egg-xlx-flash?branch=master
[david-image]: https://img.shields.io/david/eggjs/egg-xlx-flash.svg?style=flat-square
[david-url]: https://david-dm.org/eggjs/egg-xlx-flash
[snyk-image]: https://snyk.io/test/npm/egg-xlx-flash/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/egg-xlx-flash
[download-image]: https://img.shields.io/npm/dm/egg-xlx-flash.svg?style=flat-square
[download-url]: https://npmjs.org/package/egg-xlx-flash

<!--
Description here.
-->

## Install

```bash
$ npm i egg-xlx-flash --S
```

## Usage

```js
// {app_root}/config/plugin.js
exports.flash = {
    enable: true,
    package: 'egg-msg-flash'
}
```

## Configuration

```js
// {app_root}/config/config.default.js
exports.flash = {
    key: 'flash'
}
```

see [config/config.default.js](config/config.default.js) for more detail.

## Example

<!-- example here -->

```
ctx.flash = {
    type: 'success',
    message: {
        some: 'one'
    }
}

// or

ctx.flash_success({some:'one'})

ctx.flash_error()
ctx.flash_info()
ctx.flash_warning()

ctx.request.flash(type, message)

// get message by

ctx.flash
```

## Questions & Suggestions

Please open an issue [here](https://github.com/eggjs/egg/issues).

## License

[MIT](LICENSE)
