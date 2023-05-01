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

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute an integer [binary logarithm][binary-logarithm].

<section class="intro">

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import log2Uint32 from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-fast-uint32-log2@esm/index.mjs';
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

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import log2Uint32 from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-fast-uint32-log2@esm/index.mjs';

var v;
var i;

for ( i = 1; i < 101; i++ ) {
    v = log2Uint32( i >>> 0 );
    console.log( 'log2(%d) ≈ %d', i, v );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/log2`][@stdlib/math/base/special/log2]</span><span class="delimiter">: </span><span class="description">binary logarithm (base 2).</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-fast-uint32-log2.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-fast-uint32-log2

[test-image]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-fast-uint32-log2/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-fast-uint32-log2?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-fast-uint32-log2.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-fast-uint32-log2/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-fast-uint32-log2/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-fast-uint32-log2/main/LICENSE

[binary-logarithm]: https://en.wikipedia.org/wiki/Binary_logarithm

<!-- <related-links> -->

[@stdlib/math/base/special/log2]: https://github.com/stdlib-js/math-base-special-log2/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
