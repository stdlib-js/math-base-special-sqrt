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

# Square Root

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the principal [square root][square-root] of a double-precision floating-point number.

<section class="intro">

The principal [square root][square-root] is defined as

<!-- <equation class="equation" label="eq:principal_square_root" align="center" raw="\sqrt{x^2} = \begin{matrix} x, & \textrm{if}\ x \geq 0\end{matrix}" alt="Principal square root"> -->

<div class="equation" align="center" data-raw-text="\sqrt{x^2} = \begin{matrix} x, &amp; \textrm{if}\ x \geq 0\end{matrix}" data-equation="eq:principal_square_root">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/sqrt/docs/img/equation_principal_square_root.svg" alt="Principal square root">
    <br>
</div>

<!-- </equation> -->

</section>

<!-- /.intro -->



<section class="usage">

## Usage

To use in Observable,

```javascript
sqrt = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-sqrt@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var sqrt = require( 'path/to/vendor/umd/math-base-special-sqrt/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-sqrt@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.sqrt;
})();
</script>
```

#### sqrt( x )

Computes the principal [square root][square-root] of a double-precision floating-point number.

```javascript
var v = sqrt( 4.0 );
// returns 2.0

v = sqrt( 9.0 );
// returns 3.0

v = sqrt( 0.0 );
// returns 0.0

v = sqrt( NaN );
// returns NaN
```

For negative numbers, the principal [square root][square-root] is **not** defined.

```javascript
var v = sqrt( -4.0 );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-round@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-sqrt@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var x;
var i;

for ( i = 0; i < 100; i++ ) {
    x = round( randu() * 100.0 );
    console.log( 'sqrt(%d) = %d', x, sqrt( x ) );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math/base/special/cbrt`][@stdlib/math/base/special/cbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root of a double-precision floating-point number.</span>
-   <span class="package-name">[`@stdlib/math/base/special/rsqrt`][@stdlib/math/base/special/rsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root of a double-precision floating-point number.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-sqrt.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-sqrt

[test-image]: https://github.com/stdlib-js/math-base-special-sqrt/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-sqrt/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-sqrt/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-sqrt?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-sqrt.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-sqrt/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-sqrt/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-sqrt/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-sqrt/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-sqrt/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-sqrt/main/LICENSE

[square-root]: https://en.wikipedia.org/wiki/Square_root

<!-- <related-links> -->

[@stdlib/math/base/special/cbrt]: https://github.com/stdlib-js/math-base-special-cbrt/tree/umd

[@stdlib/math/base/special/rsqrt]: https://github.com/stdlib-js/math-base-special-rsqrt/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
