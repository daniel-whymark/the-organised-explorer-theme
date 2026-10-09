# The Organised Explorer

A fork of [Ghost](http://github.com/tryghost/ghost/)'s [Source](https://github.com/TryGhost/Source) theme for the [_The Organised Explorer_](https://theorganisedexplorer.com/) website.

Along with using the brand colour scheme, this theme also includes a few visual tweaks for a pleasant modern, yet minimal, experience.

&nbsp;

# Development

Source styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/) and [pnpm](https://pnpm.io/). After that, from the theme's root directory:

```bash
# install dependencies
pnpm install

# run development server
pnpm dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
pnpm zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.


# SVG Icons

Source uses inline SVG icons, included via Handlebars partials. You can find all icons inside `/partials/icons`. To use an icon just include the name of the relevant file, eg. To include the SVG icon in `/partials/icons/rss.hbs` - use `{{> "icons/rss"}}`.

You can add your own SVG icons in the same manner.

# Copyright & License

Copyright (c) 2013-2026 Ghost Foundation - Released under the [MIT license](LICENSE).
