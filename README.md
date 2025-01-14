[![npm version](https://badge.fury.io/js/%40mochajs%2Fjson-file-reporter.svg)](https://badge.fury.io/js/%40mochajs%2Fjson-file-reporter)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

# @es-joy/json-file-reporter
JSON file reporter for Mocha

A fork of `@mochajs/json-file-reporter`.

## Installation
```sh
$ npm i -D @es-joy/json-file-reporter
```

## Usage
Use `--reporter` in your test command.

```json
{
  "scripts": {
    "test": "mocha --reporter @es-joy/json-file-reporter"
  }
}
```

Or, add `reporter` to your configuration file.

```json
{
  "reporter": "@es-joy/json-file-reporter"
}
```

## Options
### output
By default, it will output to `report.json`. To write to other file, use `--reporter-options` in your test command.

```json
{
  "scripts": {
    "test": "mocha --reporter @es-joy/json-file-reporter --reporter-options output=filename.json"
  }
}
```

Or, add `reporter-option` to your configuration file.

```json
{
  "reporter": "@es-joy/json-file-reporter",
  "reporter-option": [
    "output=filename.json"
  ]
}
```
