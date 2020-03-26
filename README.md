# @jjwesterkamp/sass-utils [![npm version](https://badge.fury.io/js/%40jjwesterkamp%2Fsass-utils.svg)](https://badge.fury.io/js/%40jjwesterkamp%2Fsass-utils)
**Generic SCSS utilities for web projects.** This package provides several utilities in the form of sass mixins that help with writing common repetitive CSS rule sets. [View changelog](https://github.com/JJWesterkamp/sass-utils/blob/master/CHANGELOG.md).
## Installation

Install the package from npm:

```
$ npm install --save-dev @jjwesterkamp/sass-utils
```

## Usage


### 1. Setup required SCSS variables

A few variables are required by this package. Copy [the config file](scss/config.scss) into your project, and modify the variables to your needs. Then import it into your SCSS project:

```scss
@import 'sass-utils.config';
```

### 2. Import functions & mixins

To get started quickly import the index files importing all functions and mixins:

```scss
@import 'sass-utils.config';

@import '~@jjwesterkamp/sass-utils/scss/functions.index';
@import '~@jjwesterkamp/sass-utils/scss/mixins.index';
```

Alternatively you may import only the specific mixins that you need:

```scss
@import "~@jjwesterkamp/sass-utils/scss/mixins/absolute-block-pseudo";
@import "~@jjwesterkamp/sass-utils/scss/mixins/absolute-overlay";
@import "~@jjwesterkamp/sass-utils/scss/mixins/autofill-style";
// ...
```

## License

The MIT licence (MIT). See the [license file](https://github.com/JJWesterkamp/sass-utils/blob/master/LICENSE) for more information.
