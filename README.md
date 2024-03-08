# Basic template with Eleventy, LiquidJS & Sass processing

## Folder structure

- pages in /src
- Sass files in /src/sass
- layouts in /src/_layouts
- includes in /src/_includes
- Json files in /src/_data
- images & JavaScripts in /assets

## Page layout

- _layouts/base.liquid: head code + DecapCMS scripts
- _layouts/default.liquid: HTML5 structure
- _includes/header.liquid with Primary navigation
- _includes/aside.liquid with Secondary navigation
- _includes/footer.liquid

## Responsive navbar

- responsive mobile menu with CSS without JavaScript from [LogRocket](https://blog.logrocket.com/create-responsive-mobile-menu-with-css-no-javascript/), without classes
- add tags: primary in frontmatter

## Package.json scripts

- "watch:eleventy": "npx @11ty/eleventy --serve",
- "watch:sass": "npx sass src/sass:_site/assets/css --watch",
- "start": "npm run watch:eleventy & npm run watch:sass",
- "build": "sass src/sass:_site/assets/css --style=compressed && eleventy",
- "debug": "DEBUG=* eleventy"

## Dependencies

- "@11ty/eleventy": "^2.0.1",
- "sass": "^1.71.1"
- ready for [Decap CMS](https://decapcms.org/) integration.
