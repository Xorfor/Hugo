# Partials

These partials create the following components for a Bootstrap website:

## `head`
The [`head`](head.html) part of the HTML page contains
- `meta charset`<br/>The language will be used as defined as `LanguageCode` in [config.toml](/config/config.toml)
- `title`<br/>On the home page, the title will be the "site title" (`title` as specified in [config.toml](/config/config.toml)), on other pages it will be the "page title - site title", where "page title" is the `title` in the front matter section.
- `keywords`<br/>As specified in `keywords`in the front matter section.
- `meta name` settings as defined in [meta_name.html](meta_name.html)
- `meta property` settings as defined in [meta_property.html](meta_property.html)
- settings for stylesheet(s) as defined in [css.html](css.html).<br/>Timestamps are added with `?v=` to force the browser to refresh the cache.<br/>For Bootstrap, the used versions are specified in [config.toml](/config/config.toml) as:
    - `bootstrapVersion`, which can be something like '5', or '5.1'.
    - `iconsVersion`, which is the used version for the icon library.
- `favicon` as specified in [favicon.html](favicon.html).<br/>Timestamp is added with `?v=` to force the browser to refresh the cache.

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
