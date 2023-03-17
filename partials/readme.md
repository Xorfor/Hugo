# Partials

These partials create the following components for a Bootstrap website:

## `head`
The [`head`](head.html) part of the HTML page contains
- `meta charset`<br/>The language will be used as defined in [config.toml](/config/config.toml)
- `title` 
- `keywords`
- `meta name` settings as defined in [meta_name.html](meta_name.html)
- `meta property` settings as defined in [meta_property.html](meta_property.html)
- settings for stylesheet(s) as defined in [css.html](css.html)
- `favicon` as specified in [favicon.html](favicon.html)

This will result in the following HTML:

```
<head>
    <meta charset="utf-8">
    <title>...</title>
    <meta name="keywords" content="...,...">
    <meta name="robots" content="noindex, nofollow">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="...">
    <meta name="author" content="...">
    <meta property="og:site_name" content="..." />
    <meta property="og:description" content="..." />
    <meta property="og:locale" content="nl" />
    <meta property="og:type" content="website" />
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css?v=20230317214252">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1/font/bootstrap-icons.css?v=20230317214252">
    <link rel="stylesheet" href="./css/bb.css?v=20230317214252">
    <link rel="icon" href="./favicon.png?v=20230317214252" type="image/png">
</head>
```
