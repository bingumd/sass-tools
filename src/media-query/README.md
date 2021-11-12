# @bingumd/sass-tools/src/media-query

### function: `mq()`

Apply a media query defined in [config.scss](../config.scss).

### Arguments

| Name | Description | Type | Default |
| - | - | - | - |
| `$value` | breakpoint name | `String` | - |


### Use
```scss
@use '@bingumd/sass-tools' as tools;

.class-name {
    margin: 10px;

    @include tools.mq('md') {
        margin: 20px;
    }

    @include tools.mq('lg') {
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
