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

# FLOAT32_MAX_SAFE_INTEGER

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Maximum safe [single-precision floating-point][ieee754] integer.



<section class="usage">

## Usage

To use in Observable,

```javascript
FLOAT32_MAX_SAFE_INTEGER = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-float32-max-safe-integer@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var FLOAT32_MAX_SAFE_INTEGER = require( 'path/to/vendor/umd/constants-float32-max-safe-integer/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-float32-max-safe-integer@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.FLOAT32_MAX_SAFE_INTEGER;
})();
</script>
```

#### FLOAT32_MAX_SAFE_INTEGER

The maximum [safe][safe-integers] [single-precision floating-point][ieee754] integer.

```javascript
var bool = ( FLOAT32_MAX_SAFE_INTEGER === 16777215 );
// returns true
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
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-pow@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-float32-max-safe-integer@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var max;
var x;
var i;

max = pow( 2.0, 26 );
for ( i = 0; i < 100; i++ ) {
    x = round( randu() * max );
    if ( x > FLOAT32_MAX_SAFE_INTEGER ) {
        console.log( 'Unsafe: %d', x );
    } else {
        console.log( 'Safe: %d', x );
    }
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

-   <span class="package-name">[`@stdlib/constants/float16/max-safe-integer`][@stdlib/constants/float16/max-safe-integer]</span><span class="delimiter">: </span><span class="description">maximum safe half-precision floating-point integer.</span>
-   <span class="package-name">[`@stdlib/constants/float32/min-safe-integer`][@stdlib/constants/float32/min-safe-integer]</span><span class="delimiter">: </span><span class="description">minimum safe single-precision floating-point integer.</span>
-   <span class="package-name">[`@stdlib/constants/float64/max-safe-integer`][@stdlib/constants/float64/max-safe-integer]</span><span class="delimiter">: </span><span class="description">maximum safe double-precision floating-point integer.</span>

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

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-float32-max-safe-integer.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-float32-max-safe-integer

[test-image]: https://github.com/stdlib-js/constants-float32-max-safe-integer/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/constants-float32-max-safe-integer/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-float32-max-safe-integer/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-float32-max-safe-integer?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-float32-max-safe-integer.svg
[dependencies-url]: https://david-dm.org/stdlib-js/constants-float32-max-safe-integer/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/constants-float32-max-safe-integer/tree/deno
[umd-url]: https://github.com/stdlib-js/constants-float32-max-safe-integer/tree/umd
[esm-url]: https://github.com/stdlib-js/constants-float32-max-safe-integer/tree/esm
[branches-url]: https://github.com/stdlib-js/constants-float32-max-safe-integer/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-float32-max-safe-integer/main/LICENSE

[safe-integers]: http://www.2ality.com/2013/10/safe-integers.html

[ieee754]: https://en.wikipedia.org/wiki/IEEE_754-1985

<!-- <related-links> -->

[@stdlib/constants/float16/max-safe-integer]: https://github.com/stdlib-js/constants-float16-max-safe-integer/tree/umd

[@stdlib/constants/float32/min-safe-integer]: https://github.com/stdlib-js/constants-float32-min-safe-integer/tree/umd

[@stdlib/constants/float64/max-safe-integer]: https://github.com/stdlib-js/constants-float64-max-safe-integer/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
