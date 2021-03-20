# @bingumd/sass-utils

### function: `strip-unit()`

A small function to remove the units from a given value.

### Arguments

| Name | Description | Type | Default       |
| - | - | - | - |
| `$value` | value to be remove the unit | `Number` | - |


### Use
```scss
@use '@bingumd/sass-utils' as util;

$result: util.strip-unit(18px) // => 18
$result: util.strip-unit(33.333%) // => 33.333
```
