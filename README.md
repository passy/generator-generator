# Yeoman Generator for Yeoman Generators
[![Build Status](https://secure.travis-ci.org/yeoman/generator-generator.png?branch=master)](https://travis-ci.org/yeoman/generator-generator)

![Yo dawg, I heard you like generators?](http://i.imgur.com/2gqiift.jpg)

`generator-generator` scaffolds out a new basic Yeoman generator with some
sensible defaults.

## Commands

* `yo generator:app` shows a wizard for generating a new generator
* `yo generator:subgenerator NAME` generates a subgenerator with the name NAME

## How is this different from the built-in generator?

The built-in `yo generator` command only generates an `index.js` file for you.
`generator-generator` instead comes with a full project directory structure:

    .
    ├── app
    │   ├── index.js
    │   └── templates
    │       ├── editorconfig
    │       └── jshintrc
    ├── .editorconfig
    ├── .gitattributes
    ├── .gitignore
    ├── .jshintrc
    ├── LICENSE
    ├── package.json
    ├── README.md
    └── test
        ├── test-creation.js
        └── test-load.js

Last but not least, you don't need to copy-paste the ASCII Art Yeoman anymore.
It's already there! \o/

## Getting started
- Make sure you have [yo](https://github.com/yeoman/yo) installed:
    `npm install -g yo`
- Install the generator: `npm install -g generator-generator`
- Run: `yo generator:app` (Be sure to include `:app` as `generator` alone is part of yeoman itself.)

## Changelog

* 0.2
    * Added subgenerator for subgenerators
    * Generated generator now generates package.json, component.json and
      installs them by default.

* 0.1.1
    * Upgraded mocha to 1.9.0
    * Include `.travis.yml`

## License
[MIT License](http://en.wikipedia.org/wiki/MIT_License) |
(c) [Pascal Hartig](http://passy.me)
