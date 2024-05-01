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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Assert

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Assertion utilities.

<section class="installation">

## Installation

```bash
npm install @devtea2027/accusamus-aspernatur-voluptatibus-eos
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var assert = require( '@devtea2027/accusamus-aspernatur-voluptatibus-eos' );
```

#### assert

Namespace providing utilities for data type testing and feature detection.

```javascript
var o = assert;
// returns {...}
```

To validate the built-in JavaScript data types, the namespace includes the following assertion utilities:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array.</span>
-   <span class="signature">[`isBoolean( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boolean]</span><span class="delimiter">: </span><span class="description">test if a value is a boolean.</span>
-   <span class="signature">[`isDateObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-date-object]</span><span class="delimiter">: </span><span class="description">test if a value is a Date object.</span>
-   <span class="signature">[`isFunction( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-function]</span><span class="delimiter">: </span><span class="description">test if a value is a function.</span>
-   <span class="signature">[`isnan( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nan]</span><span class="delimiter">: </span><span class="description">test if a value is NaN.</span>
-   <span class="signature">[`isNull( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-null]</span><span class="delimiter">: </span><span class="description">test if a value is null.</span>
-   <span class="signature">[`isNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number.</span>
-   <span class="signature">[`isObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object]</span><span class="delimiter">: </span><span class="description">test if a value is an object.</span>
-   <span class="signature">[`isRegExp( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-regexp]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression.</span>
-   <span class="signature">[`isString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-string]</span><span class="delimiter">: </span><span class="description">test if a value is a string.</span>
-   <span class="signature">[`isSymbol( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symbol]</span><span class="delimiter">: </span><span class="description">test if a value is a symbol.</span>
-   <span class="signature">[`isUndefined( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-undefined]</span><span class="delimiter">: </span><span class="description">test if a value is undefined.</span>

</div>

<!-- </toc> -->

For primitive types having corresponding object wrappers, assertion utilities provide `isObject` and `isPrimitive` methods to test for either objects or primitives, respectively.

<!-- eslint-disable no-new-wrappers -->

```javascript
var Boolean = require( '@stdlib/boolean/ctor' );
var isBoolean = require( '@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boolean' );

var bool = isBoolean.isObject( new Boolean( false ) );
// returns true

bool = isBoolean.isObject( false );
// returns false

bool = isBoolean.isPrimitive( false );
// returns true
```

Many of the assertion utilities have corresponding packages that test whether array elements are of the given data type:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|nan|number|object|regexp|symbol|null|undefined)-array" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArrayArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of arrays.</span>
-   <span class="signature">[`isBooleanArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boolean-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of booleans.</span>
-   <span class="signature">[`isDateObjectArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-date-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only Date objects.</span>
-   <span class="signature">[`isFunctionArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-function-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only functions.</span>
-   <span class="signature">[`isNaNArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nan-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only NaN values.</span>
-   <span class="signature">[`isNullArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-null-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only null values.</span>
-   <span class="signature">[`isNumberArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of numbers.</span>
-   <span class="signature">[`isObjectArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only objects.</span>
-   <span class="signature">[`isStringArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-string-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of strings.</span>
-   <span class="signature">[`isSymbolArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symbol-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only symbols.</span>

</div>

<!-- </toc> -->

Where applicable, similar to the assertion utilities for built-in data types, array assertion utilities provides methods for testing for an array of primitives or objects.

<!-- eslint-disable no-new-wrappers -->

```javascript
var isStringArray = require( '@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-string-array' );

var bool = isStringArray( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.primitives( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.objects( [ 'hello', 'world' ] );
// returns false

bool = isStringArray.objects( [ new String( 'hello' ), new String( 'world' ) ] );
// returns true
```

The namespace also contains utilities to test for numbers within a certain range or for numbers satisfying a particular "type":

<!-- <toc pattern="is-*+(number|integer)*" ignore="is-number-array" ignore="is-number" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCubeNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-cube-number]</span><span class="delimiter">: </span><span class="description">test if a value is a cube number.</span>
-   <span class="signature">[`isIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only integers.</span>
-   <span class="signature">[`isInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having an integer value.</span>
-   <span class="signature">[`isNegativeIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative integers.</span>
-   <span class="signature">[`isNegativeInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative integer value.</span>
-   <span class="signature">[`isNegativeNumberArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative numbers.</span>
-   <span class="signature">[`isNegativeNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative value.</span>
-   <span class="signature">[`isNonNegativeIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative integers.</span>
-   <span class="signature">[`isNonNegativeInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative integer value.</span>
-   <span class="signature">[`isNonNegativeNumberArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative numbers.</span>
-   <span class="signature">[`isNonNegativeNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative value.</span>
-   <span class="signature">[`isNonPositiveIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive integers.</span>
-   <span class="signature">[`isNonPositiveInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive integer value.</span>
-   <span class="signature">[`isNonPositiveNumberArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive numbers.</span>
-   <span class="signature">[`isNonPositiveNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive value.</span>
-   <span class="signature">[`isPositiveIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive integers.</span>
-   <span class="signature">[`isPositiveInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive integer value.</span>
-   <span class="signature">[`isPositiveNumberArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive numbers.</span>
-   <span class="signature">[`isPositiveNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive value.</span>
-   <span class="signature">[`isSafeIntegerArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-safe-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only safe integers.</span>
-   <span class="signature">[`isSafeInteger( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-safe-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a safe integer value.</span>
-   <span class="signature">[`isSquareNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square number.</span>
-   <span class="signature">[`isSquareTriangularNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square triangular number.</span>
-   <span class="signature">[`isTriangularNumber( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a triangular number.</span>

</div>

<!-- </toc> -->

The namespace provides utilities for validating typed arrays:

<!-- <toc pattern="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array"> -->

<div class="namespace-toc">

-   <span class="signature">[`isFloat32Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float32Array.</span>
-   <span class="signature">[`isFloat64Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float64Array.</span>
-   <span class="signature">[`isInt16Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int16array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int16Array.</span>
-   <span class="signature">[`isInt32Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int32array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int32Array.</span>
-   <span class="signature">[`isInt8Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int8array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int8Array.</span>
-   <span class="signature">[`isUint16Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint16array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint16Array.</span>
-   <span class="signature">[`isUint32Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint32Array.</span>
-   <span class="signature">[`isUint8Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint8array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8Array.</span>
-   <span class="signature">[`isUint8ClampedArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint8clampedarray]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8ClampedArray.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating `ndarray`s (n-dimensional arrays).

<!-- <toc keywords="+ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCentrosymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a centrosymmetric matrix.</span>
-   <span class="signature">[`isComplex128MatrixLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128ndarrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128VectorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64MatrixLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64ndarrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64VectorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isFloat32MatrixLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32ndarrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32VectorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64MatrixLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64ndarrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64VectorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isMatrixLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is 2-dimensional ndarray-like object.</span>
-   <span class="signature">[`isndarrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is ndarray-like.</span>
-   <span class="signature">[`isNonSymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonsymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a non-symmetric matrix.</span>
-   <span class="signature">[`isPersymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a persymmetric matrix.</span>
-   <span class="signature">[`isSkewCentrosymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-centrosymmetric matrix.</span>
-   <span class="signature">[`isSkewPersymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-persymmetric matrix.</span>
-   <span class="signature">[`isSkewSymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-symmetric matrix.</span>
-   <span class="signature">[`isSquareMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object having equal dimensions.</span>
-   <span class="signature">[`isSymmetricMatrix( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a symmetric matrix.</span>
-   <span class="signature">[`isVectorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating complex numbers and arrays of complex numbers:

<!-- <toc pattern="is-complex*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isComplexLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-like]</span><span class="delimiter">: </span><span class="description">test if a value is a complex number-like object.</span>
-   <span class="signature">[`isComplexTypedArrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is complex-typed-array-like.</span>
-   <span class="signature">[`isComplexTypedArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a complex typed array.</span>
-   <span class="signature">[`isComplex( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit or 128-bit complex number.</span>
-   <span class="signature">[`isComplex128( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128]</span><span class="delimiter">: </span><span class="description">test if a value is a 128-bit complex number.</span>
-   <span class="signature">[`isComplex128Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex128Array.</span>
-   <span class="signature">[`isComplex64( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit complex number.</span>
-   <span class="signature">[`isComplex64Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex64Array.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating other special arrays or buffers:

<!-- <toc pattern="is-*array*" ignore="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array" ignore="is-*+(number|integer)*" ignore="is-+(array|boolean|date-object|function|string|nan|number|object|primitive|regexp|symbol|null|undefined)-array" ignore="is-array" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isAccessorArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object supporting the accessor (get/set) protocol.</span>
-   <span class="signature">[`isArrayLength( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid array length.</span>
-   <span class="signature">[`isArrayLikeObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>
-   <span class="signature">[`isArrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>
-   <span class="signature">[`isArrayBufferView( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arraybuffer-view]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer view.</span>
-   <span class="signature">[`isArrayBuffer( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer.</span>
-   <span class="signature">[`isBetweenArray( value, a, b[, left, right] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-between-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object where every element is between two values.</span>
-   <span class="signature">[`isBigInt64Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-bigint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt64Array.</span>
-   <span class="signature">[`isBigUint64Array( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-biguint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigUint64Array.</span>
-   <span class="signature">[`isCircularArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-circular-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array containing a circular reference.</span>
-   <span class="signature">[`isEmptyArrayLikeObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array-like object.</span>
-   <span class="signature">[`isEmptyArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-array]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array.</span>
-   <span class="signature">[`isFalsyArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-falsy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only falsy values.</span>
-   <span class="signature">[`isFiniteArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-finite-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only finite numbers.</span>
-   <span class="signature">[`isNumericArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-numeric-array]</span><span class="delimiter">: </span><span class="description">test if a value is a numeric array.</span>
-   <span class="signature">[`isPlainObjectArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-plain-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only plain objects.</span>
-   <span class="signature">[`isProbabilityArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only probabilities.</span>
-   <span class="signature">[`isSameArray( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both generic arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex128Array( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex128array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex128Arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex64Array( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex64Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat32Array( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-float32array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float32Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat64Array( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-float64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float64Arrays and have the same values.</span>
-   <span class="signature">[`isSharedArrayBuffer( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-sharedarraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is a SharedArrayBuffer.</span>
-   <span class="signature">[`isTruthyArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-truthy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only truthy values.</span>
-   <span class="signature">[`isTypedArrayLength( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid typed array length.</span>
-   <span class="signature">[`isTypedArrayLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is typed-array-like.</span>
-   <span class="signature">[`isTypedArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a typed array.</span>
-   <span class="signature">[`isUnityProbabilityArray( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-unity-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of probabilities that sum to one.</span>

</div>

<!-- </toc> -->

To test for error objects, the namespace includes the following utilities:

<!-- <toc pattern="is-*error*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-error]</span><span class="delimiter">: </span><span class="description">test if a value is an Error object.</span>
-   <span class="signature">[`isEvalError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-eval-error]</span><span class="delimiter">: </span><span class="description">test if a value is an EvalError object.</span>
-   <span class="signature">[`isRangeError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-range-error]</span><span class="delimiter">: </span><span class="description">test if a value is a RangeError object.</span>
-   <span class="signature">[`isReferenceError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-reference-error]</span><span class="delimiter">: </span><span class="description">test if a value is a ReferenceError object.</span>
-   <span class="signature">[`isSyntaxError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-syntax-error]</span><span class="delimiter">: </span><span class="description">test if a value is a SyntaxError object.</span>
-   <span class="signature">[`isTypeError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-type-error]</span><span class="delimiter">: </span><span class="description">test if a value is a TypeError object.</span>
-   <span class="signature">[`isURIError( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uri-error]</span><span class="delimiter">: </span><span class="description">test if a value is a URIError object.</span>

</div>

<!-- </toc> -->

The namespace exposes the following constants concerning the current running process:

<!-- <toc pattern="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|big-endian|node|web-worker|windows|docker|mobile|touch-device)" > -->

<div class="namespace-toc">

-   <span class="signature">[`IS_BIG_ENDIAN`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-big-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is big endian.</span>
-   <span class="signature">[`IS_BROWSER`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-browser]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web browser.</span>
-   <span class="signature">[`IS_DARWIN`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-darwin]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Darwin.</span>
-   <span class="signature">[`IS_DOCKER`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-docker]</span><span class="delimiter">: </span><span class="description">check if the process is running in a Docker container.</span>
-   <span class="signature">[`IS_ELECTRON_MAIN`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron-main]</span><span class="delimiter">: </span><span class="description">check if the runtime is the main Electron process.</span>
-   <span class="signature">[`IS_ELECTRON_RENDERER`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron-renderer]</span><span class="delimiter">: </span><span class="description">check if the runtime is the Electron renderer process.</span>
-   <span class="signature">[`IS_ELECTRON`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron]</span><span class="delimiter">: </span><span class="description">check if the runtime is Electron.</span>
-   <span class="signature">[`IS_LITTLE_ENDIAN`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-little-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is little endian.</span>
-   <span class="signature">[`IS_MOBILE`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-mobile]</span><span class="delimiter">: </span><span class="description">check if the current environment is a mobile device.</span>
-   <span class="signature">[`IS_NODE`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node]</span><span class="delimiter">: </span><span class="description">check if the runtime is Node.js.</span>
-   <span class="signature">[`IS_TOUCH_DEVICE`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-touch-device]</span><span class="delimiter">: </span><span class="description">check if the current environment is a touch device.</span>
-   <span class="signature">[`IS_WEB_WORKER`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-web-worker]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web worker.</span>
-   <span class="signature">[`IS_WINDOWS`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-windows]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Windows.</span>

</div>

<!-- </toc> -->

To test whether a runtime environment supports certain features, the namespace includes the following utilities:

<!-- <toc pattern="has-*-support" > -->

<div class="namespace-toc">

-   <span class="signature">[`hasArrayBufferSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-arraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `ArrayBuffer` support.</span>
-   <span class="signature">[`hasArrowFunctionSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-arrow-function-support]</span><span class="delimiter">: </span><span class="description">detect native `arrow function` support.</span>
-   <span class="signature">[`hasAsyncAwaitSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-async-await-support]</span><span class="delimiter">: </span><span class="description">detect native `async`/`await` support.</span>
-   <span class="signature">[`hasAsyncIteratorSymbolSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-async-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.asyncIterator` support.</span>
-   <span class="signature">[`hasBigIntSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-bigint-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt` support.</span>
-   <span class="signature">[`hasBigInt64ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-bigint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt64Array` support.</span>
-   <span class="signature">[`hasBigUint64ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-biguint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigUint64Array` support.</span>
-   <span class="signature">[`hasClassSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-class-support]</span><span class="delimiter">: </span><span class="description">detect native `class` support.</span>
-   <span class="signature">[`hasDataViewSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-dataview-support]</span><span class="delimiter">: </span><span class="description">detect native `DataView` support.</span>
-   <span class="signature">[`hasDefinePropertiesSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-define-properties-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperties` support.</span>
-   <span class="signature">[`hasDefinePropertySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-define-property-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperty` support.</span>
-   <span class="signature">[`hasFloat32ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-float32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float32Array` support.</span>
-   <span class="signature">[`hasFloat64ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-float64array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float64Array` support.</span>
-   <span class="signature">[`hasFunctionNameSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-function-name-support]</span><span class="delimiter">: </span><span class="description">detect native function `name` support.</span>
-   <span class="signature">[`hasGeneratorSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-generator-support]</span><span class="delimiter">: </span><span class="description">detect native `generator function` support.</span>
-   <span class="signature">[`hasGlobalThisSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-globalthis-support]</span><span class="delimiter">: </span><span class="description">detect `globalThis` support.</span>
-   <span class="signature">[`hasInt16ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int16Array` support.</span>
-   <span class="signature">[`hasInt32ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int32Array` support.</span>
-   <span class="signature">[`hasInt8ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int8Array` support.</span>
-   <span class="signature">[`hasIteratorSymbolSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.iterator` support.</span>
-   <span class="signature">[`hasMapSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-map-support]</span><span class="delimiter">: </span><span class="description">detect native `Map` support.</span>
-   <span class="signature">[`hasNodeBufferSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-node-buffer-support]</span><span class="delimiter">: </span><span class="description">detect native `Buffer` support.</span>
-   <span class="signature">[`hasProxySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-proxy-support]</span><span class="delimiter">: </span><span class="description">detect native `Proxy` support.</span>
-   <span class="signature">[`hasSetSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-set-support]</span><span class="delimiter">: </span><span class="description">detect native `Set` support.</span>
-   <span class="signature">[`hasSharedArrayBufferSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-sharedarraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `SharedArrayBuffer` support.</span>
-   <span class="signature">[`hasSymbolSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol` support.</span>
-   <span class="signature">[`hasToStringTagSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-tostringtag-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.toStringTag` support.</span>
-   <span class="signature">[`hasUint16ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint16Array` support.</span>
-   <span class="signature">[`hasUint32ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint32Array` support.</span>
-   <span class="signature">[`hasUint8ArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8Array` support.</span>
-   <span class="signature">[`hasUint8ClampedArraySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint8clampedarray-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8ClampedArray` support.</span>
-   <span class="signature">[`hasWebAssemblySupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-wasm-support]</span><span class="delimiter">: </span><span class="description">detect native WebAssembly support.</span>
-   <span class="signature">[`hasWeakMapSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-weakmap-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakMap` support.</span>
-   <span class="signature">[`hasWeakSetSupport()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-weakset-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakSet` support.</span>

</div>

<!-- </toc> -->

The remaining namespace utilities are as follows:

<!-- <toc ignore="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" ignore="is-*+(number|integer)*" ignore="is-*array*" ignore="is-*error*" ignore="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|node|web-worker|windows)" ignore="has-*-support" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`contains( val, searchValue[, position] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/contains]</span><span class="delimiter">: </span><span class="description">test if an array-like value contains a search value.</span>
-   <span class="signature">[`deepEqual( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-equal]</span><span class="delimiter">: </span><span class="description">test for deep equality between two values.</span>
-   <span class="signature">[`deepHasOwnProp( value, path[, options] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-has-own-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path.</span>
-   <span class="signature">[`deepHasProp( value, path[, options] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-has-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path, either own or inherited.</span>
-   <span class="signature">[`hasOwnProp( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-own-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property.</span>
-   <span class="signature">[`hasProp( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property, either own or inherited.</span>
-   <span class="signature">[`hasUTF16SurrogatePairAt( string, position )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-utf16-surrogate-pair-at]</span><span class="delimiter">: </span><span class="description">test if a position in a string marks the start of a UTF-16 surrogate pair.</span>
-   <span class="signature">[`instanceOf( value, constructor )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/instance-of]</span><span class="delimiter">: </span><span class="description">test whether a value has in its prototype chain a specified constructor as a prototype property.</span>
-   <span class="signature">[`isAbsoluteHttpURI( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-http-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute HTTP(S) URI.</span>
-   <span class="signature">[`isAbsolutePath( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-path]</span><span class="delimiter">: </span><span class="description">test if a value is an absolute path.</span>
-   <span class="signature">[`isAbsoluteURI( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute URI.</span>
-   <span class="signature">[`isAccessorPropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has an accessor descriptor.</span>
-   <span class="signature">[`isAccessorProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has an accessor descriptor.</span>
-   <span class="signature">[`isAlphagram( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-alphagram]</span><span class="delimiter">: </span><span class="description">test if a value is an alphagram.</span>
-   <span class="signature">[`isAlphaNumeric( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-alphanumeric]</span><span class="delimiter">: </span><span class="description">test whether a string contains only alphanumeric characters.</span>
-   <span class="signature">[`isAnagram( str, value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-anagram]</span><span class="delimiter">: </span><span class="description">test if a value is an anagram.</span>
-   <span class="signature">[`isArguments( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arguments]</span><span class="delimiter">: </span><span class="description">test if a value is an arguments object.</span>
-   <span class="signature">[`isArrowFunction( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arrow-function]</span><span class="delimiter">: </span><span class="description">test if a value is an `arrow function`.</span>
-   <span class="signature">[`isASCII( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-ascii]</span><span class="delimiter">: </span><span class="description">test whether a character belongs to the ASCII character set and whether this is true for all characters in a provided string.</span>
-   <span class="signature">[`isBetween( value, a, b[, left, right] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-between]</span><span class="delimiter">: </span><span class="description">test if a value is between two values.</span>
-   <span class="signature">[`isBigInt( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-bigint]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt.</span>
-   <span class="signature">[`isBinaryString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-binary-string]</span><span class="delimiter">: </span><span class="description">test if a value is a binary string.</span>
-   <span class="signature">[`isBlankString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-blank-string]</span><span class="delimiter">: </span><span class="description">test if a value is a blank string.</span>
-   <span class="signature">[`isBoxedPrimitive( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boxed-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript boxed primitive.</span>
-   <span class="signature">[`isBuffer( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a Buffer object.</span>
-   <span class="signature">[`isCamelcase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-camelcase]</span><span class="delimiter">: </span><span class="description">test if a value is a camelcase string.</span>
-   <span class="signature">[`isCapitalized( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-capitalized]</span><span class="delimiter">: </span><span class="description">test if a value is a string having an uppercase first character.</span>
-   <span class="signature">[`isCircular( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-circular]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object containing a circular reference.</span>
-   <span class="signature">[`isCircular( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-circular]</span><span class="delimiter">: </span><span class="description">test if an object-like value contains a circular reference.</span>
-   <span class="signature">[`isClass( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-class]</span><span class="delimiter">: </span><span class="description">test if a value is a class.</span>
-   <span class="signature">[`isCollection( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-collection]</span><span class="delimiter">: </span><span class="description">test if a value is a collection.</span>
-   <span class="signature">[`isComposite( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-composite]</span><span class="delimiter">: </span><span class="description">test if a value is a composite number.</span>
-   <span class="signature">[`isConfigurablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-configurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is configurable.</span>
-   <span class="signature">[`isConfigurableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-configurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is configurable.</span>
-   <span class="signature">[`isConstantcase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-constantcase]</span><span class="delimiter">: </span><span class="description">test if a value is a constantcase string.</span>
-   <span class="signature">[`isCurrentYear( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-current-year]</span><span class="delimiter">: </span><span class="description">test if a value is the current year.</span>
-   <span class="signature">[`isDataPropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-data-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has a data descriptor.</span>
-   <span class="signature">[`isDataProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-data-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has a data descriptor.</span>
-   <span class="signature">[`isDataView( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-dataview]</span><span class="delimiter">: </span><span class="description">test if a value is a DataView.</span>
-   <span class="signature">[`isDigitString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-digit-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only numeric digits.</span>
-   <span class="signature">[`isDomainName( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-domain-name]</span><span class="delimiter">: </span><span class="description">test if a value is a domain name.</span>
-   <span class="signature">[`isDurationString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-duration-string]</span><span class="delimiter">: </span><span class="description">test if a value is a duration string.</span>
-   <span class="signature">[`isEmailAddress( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-email-address]</span><span class="delimiter">: </span><span class="description">test if a value is an email address.</span>
-   <span class="signature">[`isEmptyCollection( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-collection]</span><span class="delimiter">: </span><span class="description">test if a value is an empty collection.</span>
-   <span class="signature">[`isEmptyObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty object.</span>
-   <span class="signature">[`isEmptyString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-string]</span><span class="delimiter">: </span><span class="description">test if a value is an empty string.</span>
-   <span class="signature">[`isEnumerablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-enumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is enumerable.</span>
-   <span class="signature">[`isEnumerableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-enumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is enumerable.</span>
-   <span class="signature">[`isEven( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-even]</span><span class="delimiter">: </span><span class="description">test if a value is an even number.</span>
-   <span class="signature">[`isFalsy( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-falsy]</span><span class="delimiter">: </span><span class="description">test if a value is falsy.</span>
-   <span class="signature">[`isFinite( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a finite number.</span>
-   <span class="signature">[`isGeneratorObjectLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-generator-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is `generator` object-like.</span>
-   <span class="signature">[`isGeneratorObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-generator-object]</span><span class="delimiter">: </span><span class="description">test if a value is a `generator` object.</span>
-   <span class="signature">[`isgzipBuffer( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-gzip-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a gzip buffer.</span>
-   <span class="signature">[`isHexString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-hex-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only hexadecimal digits.</span>
-   <span class="signature">[`isInfinite( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-infinite]</span><span class="delimiter">: </span><span class="description">test if a value is an infinite number.</span>
-   <span class="signature">[`isInheritedProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-inherited-property]</span><span class="delimiter">: </span><span class="description">test if an object has an inherited property.</span>
-   <span class="signature">[`isIterableLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-iterable-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterable`-like.</span>
-   <span class="signature">[`isIteratorLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-iterator-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterator`-like.</span>
-   <span class="signature">[`isJSON( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-json]</span><span class="delimiter">: </span><span class="description">test if a value is a parseable JSON string.</span>
-   <span class="signature">[`isKebabcase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-kebabcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in kebab case.</span>
-   <span class="signature">[`isLeapYear( [value] )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-leap-year]</span><span class="delimiter">: </span><span class="description">test if a value corresponds to a leap year in the Gregorian calendar.</span>
-   <span class="signature">[`isLocalhost( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-localhost]</span><span class="delimiter">: </span><span class="description">test whether a value is a localhost hostname.</span>
-   <span class="signature">[`isLowercase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-lowercase]</span><span class="delimiter">: </span><span class="description">test if a value is a lowercase string.</span>
-   <span class="signature">[`isMethodIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-method-in]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name, either own or inherited.</span>
-   <span class="signature">[`isMethod( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-method]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name.</span>
-   <span class="signature">[`isMultiSlice( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-multi-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `MultiSlice`.</span>
-   <span class="signature">[`isNamedTypedTupleLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-named-typed-tuple-like]</span><span class="delimiter">: </span><span class="description">test if a value is named typed tuple-like.</span>
-   <span class="signature">[`isNativeFunction( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-native-function]</span><span class="delimiter">: </span><span class="description">test if a value is a native function.</span>
-   <span class="signature">[`isNegativeZero( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to negative zero.</span>
-   <span class="signature">[`isNodeBuiltin( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-builtin]</span><span class="delimiter">: </span><span class="description">test whether a string matches a Node.js built-in module name.</span>
-   <span class="signature">[`isNodeDuplexStreamLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-duplex-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node duplex stream-like.</span>
-   <span class="signature">[`isNodeReadableStreamLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-readable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node readable stream-like.</span>
-   <span class="signature">[`isNodeREPL()`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-repl]</span><span class="delimiter">: </span><span class="description">check if running in a Node.js REPL environment.</span>
-   <span class="signature">[`isNodeStreamLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node stream-like.</span>
-   <span class="signature">[`isNodeTransformStreamLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-transform-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node transform stream-like.</span>
-   <span class="signature">[`isNodeWritableStreamLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-writable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node writable stream-like.</span>
-   <span class="signature">[`isNonConfigurablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonconfigurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-configurable.</span>
-   <span class="signature">[`isNonConfigurableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonconfigurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-configurable.</span>
-   <span class="signature">[`isNonEnumerablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonenumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-enumerable.</span>
-   <span class="signature">[`isNonEnumerableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonenumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-enumerable.</span>
-   <span class="signature">[`isNonNegativeFinite( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative finite value.</span>
-   <span class="signature">[`isObjectLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is object-like.</span>
-   <span class="signature">[`isOdd( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-odd]</span><span class="delimiter">: </span><span class="description">test if a value is an odd number.</span>
-   <span class="signature">[`isPascalcase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-pascalcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in Pascal case.</span>
-   <span class="signature">[`isPlainObject( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-plain-object]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object.</span>
-   <span class="signature">[`isPositiveZero( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to positive zero.</span>
-   <span class="signature">[`isPrime( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prime]</span><span class="delimiter">: </span><span class="description">test if a value is a prime number.</span>
-   <span class="signature">[`isPrimitive( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript primitive.</span>
-   <span class="signature">[`isPRNGLike( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prng-like]</span><span class="delimiter">: </span><span class="description">test if a value is PRNG-like.</span>
-   <span class="signature">[`isProbability( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-probability]</span><span class="delimiter">: </span><span class="description">test if a value is a probability.</span>
-   <span class="signature">[`isPropertyKey( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-property-key]</span><span class="delimiter">: </span><span class="description">test whether a value is a property key.</span>
-   <span class="signature">[`isPrototypeOf( obj, prototype )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prototype-of]</span><span class="delimiter">: </span><span class="description">test if an object's prototype chain contains a provided prototype.</span>
-   <span class="signature">[`isReadOnlyPropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is read-only.</span>
-   <span class="signature">[`isReadOnlyProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is read-only.</span>
-   <span class="signature">[`isReadWritePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-write-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable and writable.</span>
-   <span class="signature">[`isReadWriteProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-write-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable and writable.</span>
-   <span class="signature">[`isReadablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-readable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable.</span>
-   <span class="signature">[`isReadableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-readable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable.</span>
-   <span class="signature">[`isRegExpString( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-regexp-string]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression string.</span>
-   <span class="signature">[`isRelativePath( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-relative-path]</span><span class="delimiter">: </span><span class="description">test if a value is a relative path.</span>
-   <span class="signature">[`isRelativeURI( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-relative-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is a relative URI.</span>
-   <span class="signature">[`isSameComplex128( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex128]</span><span class="delimiter">: </span><span class="description">test if two arguments are both double-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameComplex64( v1, v2 )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex64]</span><span class="delimiter">: </span><span class="description">test if two arguments are both single-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameNativeClass( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-native-class]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same native class.</span>
-   <span class="signature">[`isSameType( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-type]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same type.</span>
-   <span class="signature">[`isSameValueZero( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-value-zero]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSameValue( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-value]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSemVer( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-semver]</span><span class="delimiter">: </span><span class="description">test if a value is a semantic version string.</span>
-   <span class="signature">[`isSlice( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `Slice`.</span>
-   <span class="signature">[`isSnakecase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-snakecase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in snake case.</span>
-   <span class="signature">[`isStartcase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-startcase]</span><span class="delimiter">: </span><span class="description">test if a value is a startcase string.</span>
-   <span class="signature">[`isStrictEqual( a, b )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-strict-equal]</span><span class="delimiter">: </span><span class="description">test if two arguments are strictly equal.</span>
-   <span class="signature">[`isTruthy( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-truthy]</span><span class="delimiter">: </span><span class="description">test if a value is truthy.</span>
-   <span class="signature">[`isUNCPath( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-unc-path]</span><span class="delimiter">: </span><span class="description">test if a value is a UNC path.</span>
-   <span class="signature">[`isUndefinedOrNull( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-undefined-or-null]</span><span class="delimiter">: </span><span class="description">test if a value is undefined or null.</span>
-   <span class="signature">[`isUppercase( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uppercase]</span><span class="delimiter">: </span><span class="description">test if a value is an uppercase string.</span>
-   <span class="signature">[`isURI( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uri]</span><span class="delimiter">: </span><span class="description">test if a value is a URI.</span>
-   <span class="signature">[`isWhitespace( value )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-whitespace]</span><span class="delimiter">: </span><span class="description">test whether a string contains only white space characters.</span>
-   <span class="signature">[`isWritablePropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-writable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is writable.</span>
-   <span class="signature">[`isWritableProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-writable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is writable.</span>
-   <span class="signature">[`isWriteOnlyPropertyIn( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-write-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is write-only.</span>
-   <span class="signature">[`isWriteOnlyProperty( value, property )`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-write-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is write-only.</span>
-   <span class="signature">[`tools`][@devtea2027/accusamus-aspernatur-voluptatibus-eos/tools]</span><span class="delimiter">: </span><span class="description">assertion utility tools.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var assert = require( '@devtea2027/accusamus-aspernatur-voluptatibus-eos' );

console.log( objectKeys( assert ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@devtea2027/accusamus-aspernatur-voluptatibus-eos.svg
[npm-url]: https://npmjs.org/package/@devtea2027/accusamus-aspernatur-voluptatibus-eos

[test-image]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/devtea2027/accusamus-aspernatur-voluptatibus-eos/main.svg
[coverage-url]: https://codecov.io/github/devtea2027/accusamus-aspernatur-voluptatibus-eos?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/devtea2027/accusamus-aspernatur-voluptatibus-eos.svg
[dependencies-url]: https://david-dm.org/devtea2027/accusamus-aspernatur-voluptatibus-eos/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/deno
[deno-readme]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/blob/deno/README.md
[umd-url]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/umd
[umd-readme]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/blob/umd/README.md
[esm-url]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/esm
[esm-readme]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/blob/esm/README.md
[branches-url]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/main/LICENSE

<!-- <toc-links> -->

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/contains]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/contains

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-equal]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/deep-equal

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-has-own-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/deep-has-own-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/deep-has-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/deep-has-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-own-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-own-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-utf16-surrogate-pair-at]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-utf16-surrogate-pair-at

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/instance-of]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/instance-of

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-http-uri]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-absolute-http-uri

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-path]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-absolute-path

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-absolute-uri]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-absolute-uri

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-accessor-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-accessor-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-alphagram]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-alphagram

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-alphanumeric]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-alphanumeric

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-anagram]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-anagram

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arguments]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-arguments

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arrow-function]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-arrow-function

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-ascii]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-ascii

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-between]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-between

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-bigint]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-bigint

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-binary-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-binary-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-blank-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-blank-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boxed-primitive]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-boxed-primitive

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-buffer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-buffer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-camelcase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-camelcase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-capitalized]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-capitalized

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-circular]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-circular

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-class]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-class

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-collection]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-collection

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-composite]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-composite

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-configurable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-configurable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-configurable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-configurable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-constantcase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-constantcase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-current-year]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-current-year

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-data-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-data-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-data-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-data-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-dataview]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-dataview

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-digit-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-digit-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-domain-name]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-domain-name

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-duration-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-duration-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-email-address]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-email-address

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-collection]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-empty-collection

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-empty-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-empty-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-enumerable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-enumerable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-enumerable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-enumerable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-even]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-even

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-falsy]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-falsy

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-finite]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-finite

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-generator-object-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-generator-object-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-generator-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-generator-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-gzip-buffer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-gzip-buffer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-hex-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-hex-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-infinite]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-infinite

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-inherited-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-inherited-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-iterable-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-iterable-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-iterator-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-iterator-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-json]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-json

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-kebabcase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-kebabcase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-leap-year]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-leap-year

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-localhost]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-localhost

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-lowercase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-lowercase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-method-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-method-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-method]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-method

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-multi-slice]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-multi-slice

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-named-typed-tuple-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-named-typed-tuple-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-native-function]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-native-function

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-zero]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-negative-zero

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-builtin]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-builtin

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-duplex-stream-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-duplex-stream-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-readable-stream-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-readable-stream-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-repl]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-repl

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-stream-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-stream-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-transform-stream-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-transform-stream-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node-writable-stream-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node-writable-stream-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonconfigurable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonconfigurable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonconfigurable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonconfigurable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonenumerable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonenumerable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonenumerable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonenumerable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-finite]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonnegative-finite

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-object-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-odd]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-odd

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-pascalcase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-pascalcase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-plain-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-plain-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-zero]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-positive-zero

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prime]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-prime

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-primitive]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-primitive

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prng-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-prng-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-probability]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-probability

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-property-key]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-property-key

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-prototype-of]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-prototype-of

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-only-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-read-only-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-only-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-read-only-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-write-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-read-write-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-read-write-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-read-write-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-readable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-readable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-readable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-readable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-regexp-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-regexp-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-relative-path]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-relative-path

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-relative-uri]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-relative-uri

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex128]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-complex128

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex64]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-complex64

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-native-class]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-native-class

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-type]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-type

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-value-zero]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-value-zero

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-value]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-value

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-semver]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-semver

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-slice]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-slice

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-snakecase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-snakecase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-startcase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-startcase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-strict-equal]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-strict-equal

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-truthy]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-truthy

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-unc-path]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-unc-path

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-undefined-or-null]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-undefined-or-null

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uppercase]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uppercase

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uri]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uri

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-whitespace]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-whitespace

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-writable-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-writable-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-writable-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-writable-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-write-only-property-in]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-write-only-property-in

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-write-only-property]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-write-only-property

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/tools]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/tools

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-arraybuffer-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-arraybuffer-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-arrow-function-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-arrow-function-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-async-await-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-async-await-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-async-iterator-symbol-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-async-iterator-symbol-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-bigint-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-bigint-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-bigint64array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-bigint64array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-biguint64array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-biguint64array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-class-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-class-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-dataview-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-dataview-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-define-properties-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-define-properties-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-define-property-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-define-property-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-float32array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-float32array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-float64array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-float64array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-function-name-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-function-name-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-generator-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-generator-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-globalthis-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-globalthis-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int16array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-int16array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int32array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-int32array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-int8array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-int8array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-iterator-symbol-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-iterator-symbol-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-map-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-map-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-node-buffer-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-node-buffer-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-proxy-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-proxy-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-set-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-set-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-sharedarraybuffer-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-sharedarraybuffer-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-symbol-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-symbol-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-tostringtag-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-tostringtag-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint16array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-uint16array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint32array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-uint32array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint8array-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-uint8array-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-uint8clampedarray-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-uint8clampedarray-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-wasm-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-wasm-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-weakmap-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-weakmap-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/has-weakset-support]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/has-weakset-support

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-big-endian]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-big-endian

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-browser]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-browser

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-darwin]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-darwin

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-docker]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-docker

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron-main]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-electron-main

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron-renderer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-electron-renderer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-electron]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-electron

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-little-endian]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-little-endian

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-mobile]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-mobile

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-node]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-node

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-touch-device]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-touch-device

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-web-worker]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-web-worker

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-windows]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-windows

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-eval-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-eval-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-range-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-range-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-reference-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-reference-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-syntax-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-syntax-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-type-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-type-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uri-error]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uri-error

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-accessor-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-accessor-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-length]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-array-length

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-like-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-array-like-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-array-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arraybuffer-view]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-arraybuffer-view

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-arraybuffer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-arraybuffer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-between-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-between-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-bigint64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-bigint64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-biguint64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-biguint64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-circular-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-circular-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-array-like-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-empty-array-like-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-empty-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-empty-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-falsy-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-falsy-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-finite-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-finite-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-numeric-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-numeric-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-plain-object-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-plain-object-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-probability-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-probability-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex128array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-complex128array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-complex64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-complex64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-float32array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-float32array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-same-float64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-same-float64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-sharedarraybuffer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-sharedarraybuffer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-truthy-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-truthy-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array-length]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-typed-array-length

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-typed-array-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-typed-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-typed-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-unity-probability-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-unity-probability-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-typed-array-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex-typed-array-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex-typed-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex-typed-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex128

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex128array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex64

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-centrosymmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-centrosymmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128matrix-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex128matrix-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128ndarray-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex128ndarray-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex128vector-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex128vector-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64matrix-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex64matrix-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64ndarray-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex64ndarray-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-complex64vector-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-complex64vector-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32matrix-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float32matrix-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32ndarray-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float32ndarray-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32vector-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float32vector-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64matrix-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float64matrix-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64ndarray-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float64ndarray-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64vector-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float64vector-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-matrix-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-matrix-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-ndarray-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-ndarray-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonsymmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonsymmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-persymmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-persymmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-centrosymmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-skew-centrosymmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-persymmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-skew-persymmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-skew-symmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-skew-symmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-square-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symmetric-matrix]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-symmetric-matrix

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-vector-like]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-vector-like

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float32array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float32array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-float64array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-float64array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int16array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-int16array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int32array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-int32array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-int8array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-int8array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint16array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uint16array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint32array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uint32array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint8array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uint8array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-uint8clampedarray]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-uint8clampedarray

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-cube-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-cube-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-negative-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-negative-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-number-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-negative-number-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-negative-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-negative-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonnegative-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonnegative-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-number-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonnegative-number-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonnegative-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonnegative-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonpositive-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonpositive-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-number-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonpositive-number-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nonpositive-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nonpositive-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-positive-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-positive-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-number-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-positive-number-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-positive-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-positive-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-safe-integer-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-safe-integer-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-safe-integer]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-safe-integer

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-square-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-square-triangular-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-square-triangular-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-triangular-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-triangular-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-array-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boolean-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-boolean-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-date-object-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-date-object-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-function-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-function-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nan-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nan-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-null-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-null-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-number-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-number-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-object-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-string-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-string-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symbol-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-symbol-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-array]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-array

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-boolean]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-boolean

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-date-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-date-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-function]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-function

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-nan]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-nan

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-null]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-null

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-number]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-number

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-object]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-object

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-regexp]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-regexp

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-string]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-string

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-symbol]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-symbol

[@devtea2027/accusamus-aspernatur-voluptatibus-eos/is-undefined]: https://github.com/devtea2027/accusamus-aspernatur-voluptatibus-eos/tree/main/is-undefined

<!-- </toc-links> -->

</section>

<!-- /.links -->
