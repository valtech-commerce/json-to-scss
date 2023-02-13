# @valtech-commerce/json-to-scss

[![npm][npm-badge]][npm-url]
[![npms.io: Score][npmsio-badge]][npmsio-url]
[![libraries.io: SourceRank][librariesio-badge]][librariesio-url]
[![License: MIT][license-badge]][license-url]

> Convert a JSON to a SCSS map


## Install

```sh
$ npm install @valtech-commerce/json-to-scss
```


## Usage

```js
const jsonToScss = require('@valtech-commerce/json-to-scss');

console.log(
  jsonToScss.convert(`
    {
      "points": [
        [0, 1.2],
        [50, 1.6],
        [200, 1.8]
      ],
      "dimension": {
        "small":   600,
        "medium":  900,
        "large":  1200,
        "xlarge": 1500
      },
      "transition": {
        "hover":     100,
        "animation": 500
      },
      "color": {
        "shell": {
          "main":  "#659d32",
          "shade": "#618931"
        },
        "fruit": "#423228"
      }
    }
  `)
);

/*
$points: (
  0 1.2,
  50 1.6,
  200 1.8
);

$dimension: (
  'small': 600,
  'medium': 900,
  'large': 1200,
  'xlarge': 1500
);

$transition: (
  'hover': 100,
  'animation': 500
);

$color: (
  'shell': (
    'main': #659d32,
    'shade': #618931
  ),
  'fruit': #423228
);
*/
```

## Source

Forked from [razwan/json-to-sass-map](https://github.com/razwan/json-to-sass-map)

## License

MIT © [Valtech Canada inc.](https://www.valtech.ca/)

[npm-badge]: https://img.shields.io/npm/v/@valtech-commerce/json-to-scss?style=flat-square
[npmsio-badge]: https://img.shields.io/npms-io/final-score/@valtech-commerce/json-to-scss?style=flat-square
[librariesio-badge]: https://img.shields.io/librariesio/sourcerank/npm/@valtech-commerce/json-to-scss?style=flat-square
[license-badge]: https://img.shields.io/badge/license-MIT-green?style=flat-square

[npm-url]: https://www.npmjs.com/package/@valtech-commerce/json-to-scss
[npmsio-url]: https://npms.io/search?q=%40valtech-commerce%2Fjson-to-scss
[librariesio-url]: https://libraries.io/npm/@valtech-commerce%2Fjson-to-scss
[license-url]: https://opensource.org/licenses/MIT
