<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Binary Logarithm

> Compute an integer [binary logarithm][binary-logarithm].

<section class="intro">

</section>

<!-- /.intro -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-fast-uint32-log2
```

</section>

<section class="usage">

## Usage

```javascript
var log2Uint32 = require( '@stdlib/math-base-special-fast-uint32-log2' );
```

#### log2Uint32( x )

Returns an **approximate** [binary logarithm][binary-logarithm] of an unsigned 32-bit integer `x`.

```javascript
var v = log2Uint32( 4 >>> 0 );
// returns 2

v = log2Uint32( 8 >>> 0 );
// returns 3

v = log2Uint32( 9 >>> 0 );
// returns 3
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   This implementation provides a performance boost when an application requires only **approximate** computations for integer arguments.
-   For applications requiring high-precision, this implementation is **never** suitable.

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var log2Uint32 = require( '@stdlib/math-base-special-fast-uint32-log2' );

var v;
var i;

for ( i = 1; i < 101; i++ ) {
    v = log2Uint32( i >>> 0 );
    console.log( 'log2(%d) ≈ %d', i, v );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-fast-uint32-log2/main/LICENSE

[binary-logarithm]: https://en.wikipedia.org/wiki/Binary_logarithm

</section>

<!-- /.links -->
