# Nanoflakes - PHP

[//]: # ([![npm]&#40;https://img.shields.io/npm/v/nanoflakes&#41;]&#40;https://www.npmjs.com/package/nanoflakes&#41;)
[![GitHub issues](https://img.shields.io/github/issues/ixalsera/nanoflakes-php)](https://github.com/ixalsera/nanoflakes-php/issues)
[![License](https://img.shields.io/github/license/ixalsera/nanoflakes-php)](https://github.com/ixalsera/nanoflakes-php/tree/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fnanoflakes%2Fnanoflakes-js)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fnanoflakes%2Fnanoflakes-js)

Reference implementation of [nanoflakes](https://github.com/nanoflakes/nanoflakes) for PHP.

Licensed under the [MIT License](https://github.com/ixalsera/nanoflakes-php/blob/master/LICENSE).

### Installation

Run the following command to install the package:

```shell
composer require ixalsera/nanoflakes-php
```

### Usage

- Use `localGenerator(epoch, generatorId)` to create a local nanoflake generator.
    - You can get an epoch by calling `Date.now()` in a Node.js shell.
    - A generator ID must be in the 0-1023 range.
- Use `NanoflakeGenerator.next()` to get a new nanoflake.
- The `Nanoflake` class is the result type `NanoflakeGenerator.next()`. It can be used as-is, or getting it's raw or encoded value. It also features utility methods such as getting the creation time of the nanoflake.

### Support
