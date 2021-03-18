# @bingumd/sass-utils

Sass plugin to add a collection of mixins, helpers and tools for your saas.

### Installation

```bash
yarn add @bingumd/sass-utils
```

### Usage

```scss
@use '@bingumd/sass-utils' as util;
```

### Example

```scss
@use '@bingumd/sass-utils' as util;

body {
    font-size: util.fluid-scale((16px, 18px));
    line-height: 1.8;
    
    @include util.mq('md') {
        line-height: 2;
    }
}

ul {
    @include util.reset-list();
}

section {
    @include util.absolute(top right 50%);
}
```

### 🔨 Task list

- [ ] Add documentation
- [x] ~~Add Media Query~~

### License
This project is licensed under the [MIT](./LICENSE) License
