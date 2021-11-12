# @bingumd/sass-tools/src/color-tint

Slightly lighten a color.

### Function: 
`color-tint()`

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$color` | color to shade | `Color` | - |
| `$percentage` | percentage of `$color` in returned color | `Number` | - |
| `$start` | start color | `Color` | #000 |

### Use
```scss
@use '@bingumd/sass-tools' as tools;

$color-$tint: tools.color-tint(#000000, 1%) // => #030303
```
