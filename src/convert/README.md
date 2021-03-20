# @bingumd/sass-utils

### function: `to-px()`, `to-rem()`, `to-em()`, `to-pc()`, `to-vw()`, `to-vh()`

A small function to remove the units from a given value.

### Arguments

| Name | Description | Type | Default       |
| - | - | - | - |
| `$value` | value to be conver | `Number` | - |


### Use
```scss
@use '@bingumd/sass-utils' as util;

$result: util.to-px(18%) // => 18px
$result: util.to-rem(33.333%) // => 33.333rem
$result: util.to-em(3) // => 3em
$result: util.to-pc(50px) // => 50%
$result: util.to-vw(110px) // => 100vw
$result: util.to-vh(10) // => 10vh
```
