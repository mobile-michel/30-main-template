# Anything that can compose a website template with Eleventy, Liquid & Sass processing.

## Folder structure

- templates in /src
- layouts in /src/_layouts
- includes in /src/_includes
- Json files in /src/_data
- Sass files in /src/sass
- images & JS in /assets

## Page layout

- _layouts/base.liquid: head code + DecapCMS scripts
- _layouts/default.liquid: HTML5 structure
- _includes/navPrimary.liquid with primary navigation
- _includes/navSecondary.liquid with secondary navigation
- _includes/navFooter.liquid with footer navigation
- _includes/copyright.liquid to include in footer landmark

## Responsive navbar

- tags: add primary, secondary or footer in frontmatter

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
