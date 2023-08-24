<h1 align="center">
   <b>
        Swiper Mods<br>
    </b>
</h1>

<p align="center">Swiper tweaks and modifications</p>

<div align="center">

[![install size](https://img.shields.io/badge/dynamic/json?url=https://packagephobia.com/v2/api.json?p=swiper-mods&query=$.install.pretty&label=install%20size&style=flat-square)](https://packagephobia.now.sh/result?p=swiper-mods)
[![npm bundle size](https://img.shields.io/bundlephobia/minzip/swiper-mods?style=flat-square)](https://bundlephobia.com/package/swiper-mods@latest)
[![npm downloads](https://img.shields.io/npm/dm/swiper-mods.svg?style=flat-square)](https://npm-stat.com/charts.html?package=swiper-mods)
[![Known Vulnerabilities](https://snyk.io/test/npm/swiper-mods/badge.svg)](https://snyk.io/test/npm/swiper-mods)

</div>

## Table of Contents

- [About](#about)
- [Installation](#installation)
- [Modules](#modules)
  - [Parallax with `Z` axis](#parallax-with-z-axis)
- [Author](#author)
- [License](#license)

## About

This package contains tweaks and modifications done to [Swiper](https://www.npmjs.com/package/swiper) mostly for my personal use that I decided to publish since it could be useful to others as well.

## Installation

```bash
$ npm install swiper-mods
```

## Modules

### Parallax with `Z` axis

The default [Parallax](https://swiperjs.com/swiper-api#parallax) module supports animating along the `X` and `Y` axes but lacks support for the `Z` axis. This module adds support for the `Z` Axis.

#### Usage

Import the `Parallax` module from `swiper-mods/modules` instead of `swiper/modules`:

```js
import { Parallax } from 'swiper-mods/modules';
```

The rest of the setup process is the same as the default Parallax module.

#### Changes

This module adds two new attributes:

- `data-swiper-parallax-z-initial`: initial `Z` value in pixels.
- `data-swiper-parallax-z`: value in pixels to move the element along the `Z` axis depending on progress.

> ⚠️ Percentage values are not supported for the `Z` axis and will be treated as pixel values (e.g. "20%" works the same as "20").

#### Demo

[Japan Slider](https://rashidshamloo.github.io/japan-slider)

## Author

Rashid Shamloo (<a href="https://github.com/rashidshamloo/">github.com/rashidshamloo</a>)

## License

[MIT](LICENSE)
