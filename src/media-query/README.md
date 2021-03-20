# @bingumd/sass-utils

### function: `mq()`

Apply a media query defined in [global.scss](../_global.scss).

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$value` | breakpoint name | `String` | - |


### Use
```scss
@use '@bingumd/sass-utils';

.class-name {
    margin: 10px;

    @include util.mq('md') {
        margin: 20px;
    }

    @include util.mq('lg') {
       margin: 30px;
    }
}

// with default settings becomes:
.class-name {
    margin: 10px;

    @media (min-width: 768px) {
        margin: 20px;
    }

   @media (min-width: 1024px) {
       margin: 30px;
    }
}
```
