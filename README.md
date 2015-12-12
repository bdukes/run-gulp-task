# run-gulp-task

[![Test coverage](https://img.shields.io/coveralls/LingyuCoder/run-gulp-task.svg?style=flat-square)](https://coveralls.io/r/LingyuCoder/run-gulp-task?branch=master)
[![Build Status](https://travis-ci.org/LingyuCoder/run-gulp-task.png)](https://travis-ci.org/LingyuCoder/run-gulp-task)
[![Dependency Status](https://david-dm.org/LingyuCoder/run-gulp-task.svg)](https://david-dm.org/LingyuCoder/run-gulp-task)
[![devDependency Status](https://david-dm.org/LingyuCoder/run-gulp-task/dev-status.svg)](https://david-dm.org/LingyuCoder/run-gulp-task#info=devDependencies)
[![NPM version](http://img.shields.io/npm/v/run-gulp-task.svg?style=flat-square)](http://npmjs.org/package/run-gulp-task)
[![node](https://img.shields.io/badge/node.js-%3E=_4.0-green.svg?style=flat-square)](http://nodejs.org/download/)
[![License](http://img.shields.io/npm/l/run-gulp-task.svg?style=flat-square)](LICENSE)
[![npm download](https://img.shields.io/npm/dm/run-gulp-task.svg?style=flat-square)](https://npmjs.org/package/run-gulp-task)

Run gulp task of a gulpfile with Promise API

## Installation

```bash
$ npm install --save run-gulp-task
```

## Usage

```javascript
const runGulpTask = require('run-gulp-task');

runGulpTask('build', '/User/xyz/yourProject/gulpfile.js')
  .then(() => {
    // do something after running
  });
  .catch(e => {
    // error handling
  })
```

## Parameters

`runGulpTask(String:taskName[, String:gulpfilePath])`

| Name       | Description  | Type | Default Value |
| :-------- | :-- | :--:| :--: | :--: |
| taskName | name of the task | String | `undefined` (Required) |
| gulpfilePath | absolute path of your gulpfile | String | `path.join(process.cwd(), 'gulpfile.js')` |

## License

The MIT License (MIT)

Copyright (c) 2015

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
