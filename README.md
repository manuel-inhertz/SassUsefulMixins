# SassUsefulMixins

> All the useful mixins and functions that i use with SASS. Il'll keep this repo always updated with new stuff.

[![NPM Version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Downloads Stats][npm-downloads]][npm-url]

## Usage example

The mixins can accept arguments and do calculations. The output of this mixin (in this case) is a CSS rule and will be unfurled where ever you @include it.

```sh
@mixin my-padding-mixin($some-number) {
  padding: $some-number;
}
```

Now we use the @include directive to insert our mixin's code.

```sh
.my-module {
  @include my-padding-mixin(10px);
}
```

And here is the output CSS code.

.my-module {
  padding: 10px;
}

A function is very similar to a mixin, however the output from a function is a single value. This can be any Sass data type, including: numbers, strings, colors, booleans, or lists.

Here's how to use a function in SASS:

```sh
.my-module {
  padding: my-calculation-function(10px, 5px);
}
```

_For more examples and usage, please refer to the [Wiki][https://sass-lang.com/guide]._


## Meta

Manuel InHertz – [@manuel_inhertz](https://twitter.com/manuel_inhertz) – manuel@manuel-inhertz.com

Distributed under the GNU.v3 license. See ``LICENSE`` for more information.

[https://github.com/manuel-inhertz](https://github.com/manuel-inhertz/)
