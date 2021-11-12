# @bingumd/sass-tools/src/fluid-scale

### function: `fluid-scale()`
Linearly scale CSS properties with units based on the viewport defined in [config.scss](../config.scss).

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$value`  | Min and Max values    | `Map`    | -      |
| `$min-vw` | Minimum windows width | `Number` | 420px  |
| `$max-vw` | Maximum windows width | `Number` | 1900px |

### Use
```scss
@use '@bingumd/sass-tools' as tools;

.selector {
    font-size: tools.fluid-scale((56px, 66px));
    margin: tools.fluid-scale((15px, 30px, true)) // true - negative value;
}

// with default settings becomes:
.selector {
    font-size: clamp(56px, calc(51.4545454545px + 1.0101010101vw), 66px);
    margin: clamp((-30px), calc(-8.1818181818px - 1.5151515152vw), (-15px));
}
```
