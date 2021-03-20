# @bingumd/sass-utils

### function: `fluid-scale()`
Linearly scale CSS properties with units based on the viewport defined in [global.scss](../_global.scss).

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$value`  | Min and Max values    | `Map`    | -      |
| `$min-vw` | Minimum windows width | `Number` | 420px  |
| `$max-vw` | Maximum windows width | `Number` | 1900px |

### Use
```scss
@use '@bingumd/sass-utils';

.selector {
    font-size: util.fluid-scale((56px, 66px));
    padding: util.fluid-scale((60px, 120px));
}

// with default settings becomes:
.selector {
    font-size: clamp(56px, calc(53.1621621622px + 0.6756756757vw), 66px);
    padding: clamp(60px, calc(42.972972973px + 4.0540540541vw), 120px);
}
```
