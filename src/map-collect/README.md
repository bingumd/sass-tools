# @bingumd/sass-tools/src/map-collect/

### function: `map-collect()`

Takes multiple maps and merges them into one.

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$maps` | Any number of maps | `...Map` | - |

### Use

```scss
@use '@bingumd/sass-tools' as tools;

$red: ( red: #ce2f3f );
$blue: ( blue: #1381b3 );
$green: ( green: #87a03c );

$colors: tools.map-collect($red, $blue, $green) // => ( red: #ce2f3f, blue: #1381b3, green: #87a03c)
```
