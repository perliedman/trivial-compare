trivial-compare
===============

The simplest possible compare function that can be used with JavaScript's `Array.prototype.sort`
and any data type that gives reasonable results for the `&lt;` and `&gt;` comparison operators.

In practice, this means you can use this library to sort numbers as well as strings without caring
what the elements actually are.

I find myself dropping this tiny utility function in more or less any app I write, so now there's
a stupid npm module to stop this madness.

(As an aside, it feels weird such a function would not be part of the standard library - I sort of
hope this is a misunderstanding on my part and this library is just totally redundant, please drop
me a note if there's a better way to do this!)

## API

There's just a single function exported by this library:

`compare(a, b)`

`comapare` will return `-1` if `a &lt; b`, `1` if `a &gt; b` and `0` otherwise (if they are equal, in other words).
