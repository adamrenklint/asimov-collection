asimov-collection
================

[![NPM version](https://badge.fury.io/js/asimov-collection.png)](http://badge.fury.io/js/asimov-collection)
[![Code Climate](https://codeclimate.com/github/adamrenklint/asimov-collection.png)](https://codeclimate.com/github/adamrenklint/asimov-collection)
[![Dependency Status](https://david-dm.org/adamrenklint/asimov-collection.png?theme=shields.io)](https://david-dm.org/adamrenklint/asimov-collection)

**Collection and model classes for [asimov.js](http://asimovjs.org)**

## How to use

### Install from NPM

    $ npm install asimov-collection

### Model and Collection

The Model and Collection classes are modified versions of [Backbone](http://backbonejs.org)'s RESTful model and collection implementations, please check out their [docs](http://backbonejs.org) to learn the basics.

### FileModel

The FileModel's ```fetch()``` method will read ```attributes.path```, set the file contents as ```attributes.raw``` and call ```parseRaw (string raw)```.

### FileCollection

The ```fetch (string path)``` method will crawl the entire tree, calling ```shouldReadPath()``` before reading in each model, giving a chance to opt out from creating certain models.

---

Made by [Adam Renklint](http://adamrenklint.com), Berlin 2014. [MIT licensed](https://github.com/adamrenklint/asimov-collection/blob/master/LICENSE).
