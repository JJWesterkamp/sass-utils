# @jjwesterkamp/sass-utils
Generic SCSS function- & mixin-utilities for web projects.

[![npm version](https://badge.fury.io/js/%40jjwesterkamp%2Fsass-utils.svg)](https://badge.fury.io/js/%40jjwesterkamp%2Fsass-utils) [View changelog](https://github.com/JJWesterkamp/sass-utils/blob/master/CHANGELOG.md)

## Required SCSS variables

Some variables are required by this package. [This config file](https://github.com/JJWesterkamp/sass-utils/blob/master/sass/config.scss) is imported in both functions.scss and mixins.scss. Example: the function `rem-calc` requires a variable `$rem-base` to exist. To override the default value, define the variable before importing this package:

```scss
$rem-base: 16px;

@import '~@jjwesterkamp/sass-utils/sass/functions';
```

Overriding works the same for all variables.

### `$rem-base`

The base size for pixel-to-rem conversion using the `rem-calc()` mixin.

### `$z-indices`

This sass map maps user-defined aliases to unitless positive integers denoting corresponding z-index values. This is a dependency of he [`z-index()`](#z-index) mixin.

## Functions

```scss
@import '~@jjwesterkamp/sass-utils/sass/functions';
```

### `rem-calc()` (from [Foundation v5](https://github.com/zurb/foundation-sites/tree/V5))

This function takes a space-separated list of unitless numbers and pixel values, and converts them to `rem` values, based on the `$rem-base` variable.

```scss
// $rem-base: 16px;

@warn rem-calc($rem-base);
console> WARNING: 1rem

@warn rem-calc($rem-base (2 * $rem-base));
console> WARNING: 1rem 2rem

@warn rem-calc(8 12 16 24);
console> WARNING: 0.5rem 0.75rem 1rem 1.5rem
```


## Mixins

```scss
@import '~@jjwesterkamp/sass-utils/sass/mixins.index';
```

### `z-index()`

Use this mixin to apply a z-index value to an element by specifying a property of the `$z-indices` map.

```scss
$z-indices: (
    site-header: 5000,
);

.site-header {
    @include z-index(site-header);
}

// Output:
.site-header {
    z-index: 5000;
}
```
---
### Mixin | `absolute-block-pseudo`

```scss
@import '~@jjwesterkamp/sass-utils/sass/mixins/absolute-block-pseudo';

.crumb {
    @include absolute-block-pseudo(after, relative) {
        width: 20px;
        height: 100%;
        left: 100%;
        background-image: url("/img/arrow-right.svg");
    }
}
```

## License

The MIT licence (MIT). See the [license file](https://github.com/JJWesterkamp/sass-utils/blob/master/LICENSE) for more information.
