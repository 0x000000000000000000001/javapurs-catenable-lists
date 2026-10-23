# purescript-catenable-lists

Java port of the PureScript `catenable-lists` package. See the
[port maintenance guide](../javapurs/docs/port-maintenance.md)
for source layout, local dependency selection and JVM validation.

## JVM tests

`./bin/test` selects `catenable-lists` in the [common isolated runner](../javapurs/docs/testing.md#port-particulier), preserving this checkout and its outputs.
Use `./bin/test --help` for options and `./bin/test --clean` to rebuild the backend. The linked guide covers prerequisites, Java target/runtime settings and retained failure logs.

[![Latest release](http://img.shields.io/github/release/purescript/purescript-catenable-lists.svg)](https://github.com/purescript/purescript-catenable-lists/releases)
[![Build status](https://github.com/purescript/purescript-catenable-lists/workflows/CI/badge.svg?branch=master)](https://github.com/purescript/purescript-catenable-lists/actions?query=workflow%3ACI+branch%3Amaster)
[![Pursuit](https://pursuit.purescript.org/packages/purescript-catenable-lists/badge)](https://pursuit.purescript.org/packages/purescript-catenable-lists)

Strict catenable list implementation for PureScript.

The implementation is based on a queue data type that is backed by a
pair of lists.

See the following references for further information.

- [Simple and Efficient Purely Functional Queues and Dequeues](http://www.westpoint.edu/eecs/SiteAssets/SitePages/Faculty%20Publication%20Documents/Okasaki/jfp95queue.pdf) (Okasaki 1995)
- [Purely Functional Data Structures](http://www.cs.cmu.edu/~rwh/theses/okasaki.pdf) (Okasaki 1996)

## Installation

```bash
spago install catenable-lists
```

## Documentation

Module documentation is [published on Pursuit](http://pursuit.purescript.org/packages/purescript-catenable-lists).

## Benchmarks

![cons](benchmarks/cons.png)

![snoc](benchmarks/snoc.png)

![uncons](benchmarks/uncons.png)

![append](benchmarks/append.png)

![snoc-uncons](benchmarks/snoc-uncons.png)

![cons-uncons-n](benchmarks/cons-uncons-n.png)

![snoc-uncons-n](benchmarks/snoc-uncons-n.png)
