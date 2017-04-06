# react-malibu

React components for using the [Malibu SVG spritesheet](https://github.com/heroku/malibu).

[![Travis][build-badge]][build]
[![npm package][npm-badge]][npm]
[![Coveralls][coveralls-badge]][coveralls]

[build-badge]: https://img.shields.io/travis/user/repo/master.png?style=flat-square
[build]: https://travis-ci.org/user/repo

[npm-badge]: https://img.shields.io/npm/v/npm-package.png?style=flat-square
[npm]: https://www.npmjs.org/package/npm-package

[coveralls-badge]: https://img.shields.io/coveralls/user/repo/master.png?style=flat-square
[coveralls]: https://coveralls.io/github/user/repo


## Setup

TBD

## Usage

This package offers two components: `<MalibuSprites>` and `<MalibuIcon>`.

#### `<MalibuSprites>`

Put this component on your page only once, it fetches and displays the entire spritesheet.

#### `<MalibuIcon>`

Use this component to instantiate an icon.

```js
<MalibuIcon name='add-badge-16' size={20} fillClass='dark-gray' />
```

##### Properties

* **`name`** (required): the name of the icon. See the full list at https://hk-malibu.herokuapp.com/.
* **`size`** (default: undefined): the desired rendering size in pixels. Note that most icons come in `-16` and `-28` pixel variants. Choose the appropriate variant for the scale you wish to render at — for example, if you're rendering an icon at 12px, use the `-16` icon as the base and `12` as the `size`. If you do not specify a size, the icon's native size will be used.
* **`fillClass`** (default: purple): the desired icon fill. Must be one of
  - `purple`
  - `dark-gray`
  - `red`
  - `orange`
  - `green`
  - `blue`
