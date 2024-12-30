# JavaScript Loose Equality (==) with Null and Undefined

This code demonstrates a common pitfall in JavaScript related to loose equality (`==`) when comparing with `null` and `undefined`.

The function `foo` intends to return 0 if the input `x` is `null`, and `x + 1` otherwise. However, due to the behavior of loose equality, `undefined` is not treated the same way as `null`.  `undefined == null` evaluates to `true`, but comparing `undefined` with anything else often results in unexpected outcomes. This leads to the function returning `NaN` for `undefined` instead of a more expected behavior. 

The solution explains how to use strict equality (`===`) to improve reliability and avoid such confusion.