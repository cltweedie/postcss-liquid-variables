# PostCSS Liquid Variables

PostCSS plugin to allow use of Liquid theme variables in CSS files.

Forked from [PostCSS Shopify Settings Variables](https://github.com/bit3725/postcss-shopify-settings-variables) and adjusted slightly for use with non-Shopify Liquid templates.

```css
.foo {
  background-color: $(theme_preferences.background_colour);
}
```

Will be transformed to:

```css
.foo {
  background-color: {{ theme_preferences.background_colour }};
}
```

## Usage

```js
postcss([ require('postcss-liquid-variables') ])
```

See PostCSS docs for examples for your environment.
