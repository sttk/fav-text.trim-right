# [@fav/text.trim-right][repo-url] [![NPM][npm-img]][npm-url] [![MIT License][mit-img]][mit-url] [![Build Status][travis-img]][travis-url] [![Build Status][appveyor-img]][appveyor-url] [![Coverage status][coverage-img]][coverage-url]

Removes trailing white spaces or specified characters from a source string.

> "fav" is an abbreviation of "favorite" and also the acronym of "for all versions".
> This package is intended to support all Node.js versions and many browsers as possible.
> At least, this package supports Node.js >= v0.10 and major Web browsers: Chrome, Firefox, IE11, Edge, Vivaldi and Safari.


## Install

To install from npm:

```sh
$ npm install --save @fav/text.trim-right
```

***NOTE:*** *npm < 2.7.0 does not support scoped package, but even old version Node.js supports it. So when you use such older npm, you should download this package from [github.com][repo-url], and move it in `node_modules/@fav/text.trim-right/` directory manually.*


## Usage

For Node.js:

```js
var trimRight = require('@fav/text.trim-right');
trimRight('  abc   '); // => '  abc'
trimRight('_-abc--_-', '_-'); // => '_-abc'
```

For Web browsers:

```html
<script src="fav.text.trim-right.min.js"></script>
<script>
var trimRight = fav.text.trimRight;
trimRight('  abc   '); // => '  abc'
</script>
```


## API

### <u>trimRight(source [, chars]) : string</u>

Removes trailing white spaces or *chars* from *source*.

**NOTE:** This function doesn't check data types of the arguments, and assumes that they are given as per the specific data types.

#### Parameters:

| Parameter |  Type  | Description        |
|-----------|:------:|--------------------|
| source    | string | The source string. |
| chars     | string | The characters to be trimmed. (Optional, and white space in default.) |

#### Return:

The trimmed string.

**Type:** string


## Checked                                                                      

### Node.js (4〜9)

| Platform  |   4    |   5    |   6    |   7    |   8    |   9    |
|:---------:|:------:|:------:|:------:|:------:|:------:|:------:|
| macOS     |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|
| Windows10 |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|
| Linux     |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|

### io.js (1〜3)

| Platform  |   1    |   2    |   3    |
|:---------:|:------:|:------:|:------:|
| macOS     |&#x25ef;|&#x25ef;|&#x25ef;|
| Windows10 |&#x25ef;|&#x25ef;|&#x25ef;|
| Linux     |&#x25ef;|&#x25ef;|&#x25ef;|

### Node.js (〜0.12)

| Platform  |  0.7   |  0.8   |  0.9   |  0.10  |  0.11  |  0.12  |
|:---------:|:------:|:------:|:------:|:------:|:------:|:------:|
| macOS     |        |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|
| Windows10 |        |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|
| Linux     |&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|&#x25ef;|

### Web browsers

| Platform  | Chrome | Firefox | Vivaldi | Safari |  Edge  | IE11   |
|:---------:|:------:|:-------:|:-------:|:------:|:------:|:------:|
| macOS     |&#x25ef;|&#x25ef; |&#x25ef; |&#x25ef;|   --   |   --   |
| Windows10 |&#x25ef;|&#x25ef; |&#x25ef; |   --   |&#x25ef;|&#x25ef;|
| Linux     |&#x25ef;|&#x25ef; |&#x25ef; |   --   |   --   |   --   |


## License

Copyright (C) 2017-2018 Takayuki Sato

This program is free software under [MIT][mit-url] License.
See the file LICENSE in this distribution for more details.

[repo-url]: https://github.com/sttk/fav-text.trim-right/
[npm-img]: https://img.shields.io/badge/npm-v1.0.1-blue.svg
[npm-url]: https://www.npmjs.com/package/@fav/text.trim-right
[mit-img]: https://img.shields.io/badge/license-MIT-green.svg
[mit-url]: https://opensource.org/licenses/MIT
[travis-img]: https://travis-ci.org/sttk/fav-text.trim-right.svg?branch=master
[travis-url]: https://travis-ci.org/sttk/fav-text.trim-right
[appveyor-img]: https://ci.appveyor.com/api/projects/status/github/sttk/fav-text.trim-right?branch=master&svg=true
[appveyor-url]: https://ci.appveyor.com/project/sttk/fav-text-trim-right
[coverage-img]: https://coveralls.io/repos/github/sttk/fav-text.trim-right/badge.svg?branch=master
[coverage-url]: https://coveralls.io/github/sttk/fav-text.trim-right?branch=master
