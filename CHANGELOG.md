# Changelog

[View releases](https://github.com/JJWesterkamp/sass-utils/releases)



# v2.1.0
[v2.0.0 ... v2.1.0](https://github.com/JJWesterkamp/sass-utils/compare/v2.0.0...v2.1.0)

**Additions**

- `rem-calc()` function + required utility functions
- `z-index()` mixin to output a z-index rule with value from `$z-indices` map
- `autofill-style()` mixin to consistently override default styles on browser-autofilled inputs (webkit only)

**Changes & improvements**

- Added `@content` directives to the `placeholder-color()` mixin for easy inline extension



# v2.0.0
[v1.1.0 ... v2.0.0](https://github.com/JJWesterkamp/sass-utils/compare/v1.1.0...v2.0.0)

**Changes & improvements**

- [Breaking] Changed casing of mixin & variable names from camel-case to kebab-case



# v1.1.0 
[v1.0.0 ... v1.1.0](https://github.com/JJWesterkamp/sass-utils/compare/v1.0.0...v1.1.0)

**Additions**

- `map-deep-get()` function to get a deep value from multidimensional sass-map by giving a list of nested keys



# v1.0.0

Initial version

**Additions**

- mixin `absoluteBlockPseudo()`
- mixin `squarePseudo()`
- mixin `centered-cover-background()`
- mixin `centered-contain-background()`
- mixin `centered-flex-row()`
- mixin `centered-flex-column`
- mixin `absolute-overlay()`
- mixin `ellipsis()`
- mixin `placeholder-color()`
