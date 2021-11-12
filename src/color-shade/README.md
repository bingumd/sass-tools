# @bingumd/sass-tools/src/color-shade

Slightly darken a color.

### Function: 
`color-shade()`

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$color` | color to shade | `Color` | - |
| `$percentage` | percentage of `$color` in returned color | `Number` | - |
| `$start` | start color | `Color` | #000 |

### Use
```scss
@use '@bingumd/sass-tools' as tools;

$color-shade: tools.color-shade(#ffffff, 3%) // => #f7f7f7
```
