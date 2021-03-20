# @bingumd/sass-utils

### mixin: `position()`
Shorthand mixin for offset positioning.

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$position ` | `relative`, `absolute` or `fixed` | `String`   | - |
| `$top `      | Top offset                        | `Length ` | - |
| `$right `    | Right offset                      | `Length ` | - |
| `$bottom `   | Bottom offset                     | `Length ` | - |
| `$Left `     | Left offset                       | `Length ` | - |


### Use
```scss
@use '@bingumd/sass-utils';

.selector {
    @include util.position(absolute, right 33.333%, bottom);
}

// Output
@include true.expect {
    position: absolute;
    right: 33.333%;
    bottom: 0;
}
```

### mixin: `absolute()` and `fixed()`

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$top `      | Top offset    | `Length ` | - |
| `$right `    | Right offset  | `Length ` | - |
| `$bottom `   | Bottom offset | `Length ` | - |
| `$Left `     | Left offset   | `Length ` | - |


### Use
```scss
@use '@bingumd/sass-utils';

.selector {
    @include util.absolute(top bottom left 50px);
}

.selector {
    @include util.fixed(top 10% right);
}

// Output
.selector {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 50px
}

.selector {
    position: fixed;
    top: 10%;
    right: 0;
}
```

### mixin: `absoluteFill()` and `fixedFill()`

### Use
```scss
@use '@bingumd/sass-utils';

.selector {
    @include util.absoluteFill;
}

.selector {
    @include util.fixedFill;
}

// Output
.selector {
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
}

.selector {
    position: fixed;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
}
```
