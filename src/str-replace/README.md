# @bingumd/sass-tools/src/str-replace

### function: `str-replace()`

Replace `$search` with `$replace` in `$string`

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$string`  | Initial string       | `String` | - |
| `$search`  | Substring to replace | `String` | - |
| `$replace` | New value            | `String` | - |

### Use

```scss
@use '@bingumd/sass-tools' as tools;

$string: 'this is string';
$new-string: tools.str-replace($string, 'i', 'X'); // => thXs Xo strXng
```
