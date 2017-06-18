# @taskr/xo [![npm](https://img.shields.io/npm/v/taskr-xo.svg)](https://npmjs.org/package/taskr-xo)

> [XO](https://github.com/sindresorhus/xo) plugin for [Taskr](https://github.com/lukeed/taskr).

## Install

```
$ npm install --save-dev taskr-xo
```

## Usage

```js
exports.lint = function * (task) {
  yield task.source('test/**/*.js')
    .xo({
      semicolon: false
    })
    // ...
    .target('dist');
}
```

## API

### .xo(options)

Any options you pass in will override XO's default settings.

Read more about [configuring XO](https://github.com/sindresorhus/xo#config) for details.

#### options.quiet

Type: `boolean`<br>
Default: `false`

Report errors only.

## License

MIT © [Luke Edwards](https://lukeed.com)
