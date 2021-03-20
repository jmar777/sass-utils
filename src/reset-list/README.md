# @bingumd/sass-utils

### mixin: `reset-list()`

Reset list styles.

### Use
```scss
@use '@bingumd/sass-utils' as util;

.selector {
    @include util.reset-list;
}

// output:
.selector {
    margin: 0;
    padding: 0;
    list-stile: none;
}
```
