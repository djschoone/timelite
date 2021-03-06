# Timelite [![Build Status](https://travis-ci.org/joseluisq/timelite.svg?branch=master)](https://travis-ci.org/joseluisq/timelite)

> String time utilities with ease.

__Note:__ This project is "Work In Progress" yet.

## API

- [x] Add an array of string times. Eg. `add(['04:20:10', '21:15:10'])`
- [x] Format an array of time values into string time. Eg. `str([12, 0, 45])` > `"12:00:45"`
- [ ] Subtract an array of string times. Eg. `add(['04:20:10', '21:15:10'])`

## Install

[Yarn](https://github.com/yarnpkg/)

```sh
yarn add timelite --dev
```

[NPM](https://www.npmjs.com/)

```sh
npm install timelite --save-dev
```

## Usage

### add

Add an array of string time values "HH:mm:ss".

```js
const { add } = require('timelite')

add(['04:20:10', '21:15:10'])
// "25:35:20"
add(['04:35:10', '21:35:10'])
// "26:10:20"
add(['30:59', '17:10'])
// "48:09:00"
add(['19:30:00', '00:30:00'])
// "20:00:00"
```

### str

Format an array time values into string time.

```js
const { str } = require('timelite')

str([12, 10, 45])
// "12:10:45"
str([5, 1, 0])
// "05:01:00"
str([7, 22])
// "07:22:00"
```

## Contributions

Feel free to send some [Pull request](https://github.com/joseluisq/timelite/pulls) or [issue](https://github.com/joseluisq/timelite/issues).

## License
MIT license

© 2018 [José Luis Quintana](http://git.io/joseluisq)
