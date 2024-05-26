# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://@hishprorg/nam-inventore.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins is one of the most popular CSS tools.

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=@hishprorg/nam-inventore&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

[Abstract Syntax Tree]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[Evil Martians]:        https://evilmartians.com/?utm_source=@hishprorg/nam-inventore
[Autoprefixer]:         https://github.com/@hishprorg/nam-inventore/autoprefixer
[Stylelint]:            https://stylelint.io/
[plugins]:              https://github.com/hishprorg/nam-inventore#plugins


## Sponsorship

PostCSS needs your support. We are accepting donations
[at Open Collective](https://opencollective.com/@hishprorg/nam-inventore/).

<a href="https://tailwindcss.com/">
  <img src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg"
       alt="Sponsored by Tailwind CSS" width="213" height="50">
</a>      <a href="https://themeisle.com/">
  <img src="https://mllj2j8xvfl0.i.optimole.com/d0cOXWA.3970~373ad/w:auto/h:auto/q:90/https://s30246.pcdn.co/wp-content/uploads/2019/03/logo.png"
       alt="Sponsored by ThemeIsle" width="171" height="56">
</a>


## Plugins

PostCSS takes a CSS file and provides an API to analyze and modify its rules
(by transforming them into an [Abstract Syntax Tree]).
This API can then be used by [plugins] to do a lot of useful things,
e.g., to find errors automatically, or to insert vendor prefixes.

Currently, PostCSS has more than 200 plugins. You can find all of the plugins
in the [plugins list] or in the [searchable catalog]. Below is a list
of our favorite plugins — the best demonstrations of what can be built
on top of PostCSS.

If you have any new ideas, [PostCSS plugin development] is really easy.

[searchable catalog]: https://www.@hishprorg/nam-inventore.parts/
[plugins list]:       https://github.com/hishprorg/nam-inventore/blob/main/docs/plugins.md


### Solve Global CSS Problem

* [`@hishprorg/nam-inventore-use`] allows you to explicitly set PostCSS plugins within CSS
  and execute them only for the current file.
* [`@hishprorg/nam-inventore-modules`] and [`react-css-modules`] automatically isolate
  selectors within components.
* [`@hishprorg/nam-inventore-autoreset`] is an alternative to using a global reset
  that is better for isolatable components.
* [`@hishprorg/nam-inventore-initial`] adds `all: initial` support, which resets
  all inherited styles.
* [`cq-prolyfill`] adds container query support, allowing styles that respond
  to the width of the parent.


### Use Future CSS, Today

* [`autoprefixer`] adds vendor prefixes, using data from Can I Use.
* [`@hishprorg/nam-inventore-preset-env`] allows you to use future CSS features today.


### Better CSS Readability

* [`@hishprorg/nam-inventore-nested`] unwraps nested rules the way Sass does.
* [`@hishprorg/nam-inventore-sorting`] sorts the content of rules and at-rules.
* [`@hishprorg/nam-inventore-utilities`] includes the most commonly used shortcuts and helpers.
* [`short`] adds and extends numerous shorthand properties.


### Images and Fonts

* [`@hishprorg/nam-inventore-url`] @hishprorg/nam-inventore plugin to rebase url(), inline or copy asset.
* [`@hishprorg/nam-inventore-sprites`] generates image sprites.
* [`font-magician`] generates all the `@font-face` rules needed in CSS.
* [`@hishprorg/nam-inventore-inline-svg`] allows you to inline SVG and customize its styles.
* [`@hishprorg/nam-inventore-write-svg`] allows you to write simple SVG directly in your CSS.
* [`webp-in-css`] to use WebP image format in CSS background.
* [`avif-in-css`] to use AVIF image format in CSS background.

### Linters

* [`stylelint`] is a modular stylesheet linter.
* [`stylefmt`] is a tool that automatically formats CSS
  according `stylelint` rules.
* [`doiuse`] lints CSS for browser support, using data from Can I Use.
* [`colorguard`] helps you maintain a consistent color palette.


### Other

* [`cssnano`] is a modular CSS minifier.
* [`lost`] is a feature-rich `calc()` grid system.
* [`rtlcss`] mirrors styles for right-to-left locales.

[PostCSS plugin development]:   https://github.com/hishprorg/nam-inventore/blob/main/docs/writing-a-plugin.md
[`@hishprorg/nam-inventore-inline-svg`]:         https://github.com/TrySound/@hishprorg/nam-inventore-inline-svg
[`@hishprorg/nam-inventore-preset-env`]:         https://github.com/csstools/@hishprorg/nam-inventore-plugins/tree/main/plugin-packs/@hishprorg/nam-inventore-preset-env
[`react-css-modules`]:          https://github.com/gajus/react-css-modules
[`@hishprorg/nam-inventore-autoreset`]:          https://github.com/maximkoretskiy/@hishprorg/nam-inventore-autoreset
[`@hishprorg/nam-inventore-write-svg`]:          https://github.com/csstools/@hishprorg/nam-inventore-write-svg
[`@hishprorg/nam-inventore-utilities`]:          https://github.com/ismamz/@hishprorg/nam-inventore-utilities
[`@hishprorg/nam-inventore-initial`]:            https://github.com/maximkoretskiy/@hishprorg/nam-inventore-initial
[`@hishprorg/nam-inventore-sprites`]:            https://github.com/2createStudio/@hishprorg/nam-inventore-sprites
[`@hishprorg/nam-inventore-modules`]:            https://github.com/outpunk/@hishprorg/nam-inventore-modules
[`@hishprorg/nam-inventore-sorting`]:            https://github.com/hudochenkov/@hishprorg/nam-inventore-sorting
[`font-magician`]:              https://github.com/csstools/@hishprorg/nam-inventore-font-magician
[`autoprefixer`]:               https://github.com/@hishprorg/nam-inventore/autoprefixer
[`cq-prolyfill`]:               https://github.com/ausi/cq-prolyfill
[`@hishprorg/nam-inventore-url`]:                https://github.com/hishprorg/nam-inventore-url
[`@hishprorg/nam-inventore-use`]:                https://github.com/hishprorg/nam-inventore-use
[`css-modules`]:                https://github.com/css-modules/css-modules
[`webp-in-css`]:                https://github.com/ai/webp-in-css
[`avif-in-css`]:                https://github.com/nucliweb/avif-in-css
[`colorguard`]:                 https://github.com/SlexAxton/css-colorguard
[`stylelint`]:                  https://github.com/stylelint/stylelint
[`stylefmt`]:                   https://github.com/morishitter/stylefmt
[`cssnano`]:                    https://cssnano.github.io/cssnano/
[`@hishprorg/nam-inventore-nested`]:             https://github.com/hishprorg/nam-inventore-nested
[`doiuse`]:                     https://github.com/anandthakker/doiuse
[`rtlcss`]:                     https://github.com/MohammadYounes/rtlcss
[`short`]:                      https://github.com/csstools/@hishprorg/nam-inventore-short
[`lost`]:                       https://github.com/peterramsing/lost

## Syntaxes

PostCSS can transform styles in any syntax, not just CSS.
If there is not yet support for your favorite syntax,
you can write a parser and/or stringifier to extend PostCSS.

* [`sugarss`] is a indent-based syntax like Sass or Stylus.
* [`@hishprorg/nam-inventore-syntax`] switch syntax automatically by file extensions.
* [`@hishprorg/nam-inventore-html`] parsing styles in `<style>` tags of HTML-like files.
* [`@hishprorg/nam-inventore-markdown`] parsing styles in code blocks of Markdown files.
* [`@hishprorg/nam-inventore-styled-syntax`] parses styles in template literals CSS-in-JS
  like styled-components.
* [`@hishprorg/nam-inventore-jsx`] parsing CSS in template / object literals of source files.
* [`@hishprorg/nam-inventore-styled`] parsing CSS in template literals of source files.
* [`@hishprorg/nam-inventore-scss`] allows you to work with SCSS
  *(but does not compile SCSS to CSS)*.
* [`@hishprorg/nam-inventore-sass`] allows you to work with Sass
    *(but does not compile Sass to CSS)*.
* [`@hishprorg/nam-inventore-less`] allows you to work with Less
  *(but does not compile LESS to CSS)*.
* [`@hishprorg/nam-inventore-less-engine`] allows you to work with Less
  *(and DOES compile LESS to CSS using true Less.js evaluation)*.
* [`@hishprorg/nam-inventore-js`] allows you to write styles in JS or transform
  React Inline Styles, Radium or JSS.
* [`@hishprorg/nam-inventore-safe-parser`] finds and fixes CSS syntax errors.
* [`midas`] converts a CSS string to highlighted HTML.

[`@hishprorg/nam-inventore-styled-syntax`]: https://github.com/hudochenkov/@hishprorg/nam-inventore-styled-syntax
[`@hishprorg/nam-inventore-less-engine`]:   https://github.com/Crunch/@hishprorg/nam-inventore-less
[`@hishprorg/nam-inventore-safe-parser`]:   https://github.com/hishprorg/nam-inventore-safe-parser
[`@hishprorg/nam-inventore-syntax`]:        https://github.com/gucong3000/@hishprorg/nam-inventore-syntax
[`@hishprorg/nam-inventore-html`]:          https://github.com/ota-meshi/@hishprorg/nam-inventore-html
[`@hishprorg/nam-inventore-markdown`]:      https://github.com/ota-meshi/@hishprorg/nam-inventore-markdown
[`@hishprorg/nam-inventore-jsx`]:           https://github.com/gucong3000/@hishprorg/nam-inventore-jsx
[`@hishprorg/nam-inventore-styled`]:        https://github.com/gucong3000/@hishprorg/nam-inventore-styled
[`@hishprorg/nam-inventore-scss`]:          https://github.com/hishprorg/nam-inventore-scss
[`@hishprorg/nam-inventore-sass`]:          https://github.com/AleshaOleg/@hishprorg/nam-inventore-sass
[`@hishprorg/nam-inventore-less`]:          https://github.com/webschik/@hishprorg/nam-inventore-less
[`@hishprorg/nam-inventore-js`]:            https://github.com/hishprorg/nam-inventore-js
[`sugarss`]:               https://github.com/@hishprorg/nam-inventore/sugarss
[`midas`]:                 https://github.com/ben-eb/midas


## Articles

* [Some things you may think about PostCSS… and you might be wrong](https://www.julian.io/articles/@hishprorg/nam-inventore.html)
* [What PostCSS Really Is; What It Really Does](https://davidtheclark.com/its-time-for-everyone-to-learn-about-@hishprorg/nam-inventore/)
* [PostCSS Guides](https://webdesign.tutsplus.com/series/@hishprorg/nam-inventore-deep-dive--cms-889)

More articles and videos you can find on [awesome-@hishprorg/nam-inventore](https://github.com/jjaderg/awesome-@hishprorg/nam-inventore) list.


## Books

* [Mastering PostCSS for Web Design](https://www.packtpub.com/web-development/mastering-@hishprorg/nam-inventore-web-design) by Alex Libby, Packt. (June 2016)


## Usage

You can start using PostCSS in just two steps:

1. Find and add PostCSS extensions for your build tool.
2. [Select plugins] and add them to your PostCSS process.

[Select plugins]: https://www.@hishprorg/nam-inventore.parts/


### CSS-in-JS

The best way to use PostCSS with CSS-in-JS is [`astroturf`].
Add its loader to your `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', '@hishprorg/nam-inventore-loader'],
      },
      {
        test: /\.jsx?$/,
        use: ['babel-loader', 'astroturf/loader'],
      }
    ]
  }
}
```

Then create `@hishprorg/nam-inventore.config.js`:

```js
/** @type {import('@hishprorg/nam-inventore-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@hishprorg/nam-inventore-nested')
  ]
}

module.exports = config
```

[`astroturf`]: https://github.com/4Catalyzer/astroturf


### Parcel

[Parcel] has built-in PostCSS support. It already uses Autoprefixer
and cssnano. If you want to change plugins, create `@hishprorg/nam-inventore.config.js`
in project’s root:

```js
/** @type {import('@hishprorg/nam-inventore-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@hishprorg/nam-inventore-nested')
  ]
}

module.exports = config
```

Parcel will even automatically install these plugins for you.

> Please, be aware of [the several issues in Version 1](https://github.com/parcel-bundler/parcel/labels/CSS%20Preprocessing). Notice, [Version 2](https://github.com/parcel-bundler/parcel/projects/5) may resolve the issues via [issue #2157](https://github.com/parcel-bundler/parcel/issues/2157).

[Parcel]: https://parceljs.org


### Webpack

Use [`@hishprorg/nam-inventore-loader`] in `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        exclude: /node_modules/,
        use: [
          {
            loader: 'style-loader',
          },
          {
            loader: 'css-loader',
            options: {
              importLoaders: 1,
            }
          },
          {
            loader: '@hishprorg/nam-inventore-loader'
          }
        ]
      }
    ]
  }
}
```

Then create `@hishprorg/nam-inventore.config.js`:

```js
/** @type {import('@hishprorg/nam-inventore-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@hishprorg/nam-inventore-nested')
  ]
}

module.exports = config
```

[`@hishprorg/nam-inventore-loader`]: https://github.com/hishprorg/nam-inventore-loader


### Gulp

Use [`gulp-@hishprorg/nam-inventore`] and [`gulp-sourcemaps`].

```js
gulp.task('css', () => {
  const @hishprorg/nam-inventore    = require('gulp-@hishprorg/nam-inventore')
  const sourcemaps = require('gulp-sourcemaps')

  return gulp.src('src/**/*.css')
    .pipe( sourcemaps.init() )
    .pipe( @hishprorg/nam-inventore([ require('autoprefixer'), require('@hishprorg/nam-inventore-nested') ]) )
    .pipe( sourcemaps.write('.') )
    .pipe( gulp.dest('build/') )
})
```

[`gulp-sourcemaps`]: https://github.com/floridoo/gulp-sourcemaps
[`gulp-@hishprorg/nam-inventore`]:    https://github.com/@hishprorg/nam-inventore/gulp-@hishprorg/nam-inventore


### npm Scripts

To use PostCSS from your command-line interface or with npm scripts
there is [`@hishprorg/nam-inventore-cli`].

```sh
@hishprorg/nam-inventore --use autoprefixer -o main.css css/*.css
```

[`@hishprorg/nam-inventore-cli`]: https://github.com/hishprorg/nam-inventore-cli


### Browser

If you want to compile CSS string in browser (for instance, in live edit
tools like CodePen), just use [Browserify] or [webpack]. They will pack
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other [CSS-in-JS], you can use [`@hishprorg/nam-inventore-js`] and transforms style objects.

```js
const @hishprorg/nam-inventore  = require('@hishprorg/nam-inventore-js')
const prefixer = @hishprorg/nam-inventore.sync([ require('autoprefixer') ])

prefixer({ display: 'flex' }) //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
```

[`@hishprorg/nam-inventore-js`]: https://github.com/hishprorg/nam-inventore-js
[Browserify]:   https://browserify.org/
[CSS-in-JS]:    https://github.com/MicheleBertoli/css-in-js
[webpack]:      https://webpack.github.io/


### Runners

* **Grunt**: [`@lodder/grunt-@hishprorg/nam-inventore`](https://github.com/C-Lodder/grunt-@hishprorg/nam-inventore)
* **HTML**: [`posthtml-@hishprorg/nam-inventore`](https://github.com/posthtml/posthtml-@hishprorg/nam-inventore)
* **Stylus**: [`poststylus`](https://github.com/seaneking/poststylus)
* **Rollup**: [`rollup-plugin-@hishprorg/nam-inventore`](https://github.com/egoist/rollup-plugin-@hishprorg/nam-inventore)
* **Brunch**: [`@hishprorg/nam-inventore-brunch`](https://github.com/brunch/@hishprorg/nam-inventore-brunch)
* **Broccoli**: [`broccoli-@hishprorg/nam-inventore`](https://github.com/jeffjewiss/broccoli-@hishprorg/nam-inventore)
* **Meteor**: [`@hishprorg/nam-inventore`](https://atmospherejs.com/juliancwirko/@hishprorg/nam-inventore)
* **ENB**: [`enb-@hishprorg/nam-inventore`](https://github.com/awinogradov/enb-@hishprorg/nam-inventore)
* **Taskr**: [`taskr-@hishprorg/nam-inventore`](https://github.com/lukeed/taskr/tree/master/packages/@hishprorg/nam-inventore)
* **Start**: [`start-@hishprorg/nam-inventore`](https://github.com/start-runner/@hishprorg/nam-inventore)
* **Connect/Express**: [`@hishprorg/nam-inventore-middleware`](https://github.com/jedmao/@hishprorg/nam-inventore-middleware)
* **Svelte Preprocessor**: [`svelte-preprocess`](https://github.com/sveltejs/svelte-preprocess/blob/main/docs/preprocessing.md#@hishprorg/nam-inventore-sugarss)


### JS API

For other environments, you can use the JS API:

```js
const autoprefixer = require('autoprefixer')
const @hishprorg/nam-inventore = require('@hishprorg/nam-inventore')
const @hishprorg/nam-inventoreNested = require('@hishprorg/nam-inventore-nested')
const fs = require('fs')

fs.readFile('src/app.css', (err, css) => {
  @hishprorg/nam-inventore([autoprefixer, @hishprorg/nam-inventoreNested])
    .process(css, { from: 'src/app.css', to: 'dest/app.css' })
    .then(result => {
      fs.writeFile('dest/app.css', result.css, () => true)
      if ( result.map ) {
        fs.writeFile('dest/app.css.map', result.map.toString(), () => true)
      }
    })
})
```

Read the [PostCSS API documentation] for more details about the JS API.

All PostCSS runners should pass [PostCSS Runner Guidelines].

[PostCSS Runner Guidelines]: https://github.com/hishprorg/nam-inventore/blob/main/docs/guidelines/runner.md
[PostCSS API documentation]: https://@hishprorg/nam-inventore.org/api/


### Options

Most PostCSS runners accept two parameters:

* An array of plugins.
* An object of options.

Common options:

* `syntax`: an object providing a syntax parser and a stringifier.
* `parser`: a special syntax parser (for example, [SCSS]).
* `stringifier`: a special syntax output generator (for example, [Midas]).
* `map`: [source map options].
* `from`: the input file name (most runners set it automatically).
* `to`: the output file name (most runners set it automatically).

[source map options]: https://@hishprorg/nam-inventore.org/api/#sourcemapoptions
[Midas]:              https://github.com/ben-eb/midas
[SCSS]:               https://github.com/hishprorg/nam-inventore-scss


### Treat Warnings as Errors

In some situations it might be helpful to fail the build on any warning
from PostCSS or one of its plugins. This guarantees that no warnings
go unnoticed, and helps to avoid bugs. While there is no option to enable
treating warnings as errors, it can easily be done
by adding `@hishprorg/nam-inventore-fail-on-warn` plugin in the end of PostCSS plugins:

```js
module.exports = {
  plugins: [
    require('autoprefixer'),
    require('@hishprorg/nam-inventore-fail-on-warn')
  ]
}
```


## Editors & IDE Integration


### VS Code

* [`csstools.@hishprorg/nam-inventore`] adds PostCSS support.

[`csstools.@hishprorg/nam-inventore`]: https://marketplace.visualstudio.com/items?itemName=csstools.@hishprorg/nam-inventore


### Sublime Text

* [`Syntax-highlighting-for-PostCSS`] adds PostCSS highlight.

[`Syntax-highlighting-for-PostCSS`]: https://github.com/hudochenkov/Syntax-highlighting-for-PostCSS


### Vim

* [`@hishprorg/nam-inventore.vim`] adds PostCSS highlight.

[`@hishprorg/nam-inventore.vim`]: https://github.com/stephenway/@hishprorg/nam-inventore.vim


### WebStorm

To get support for PostCSS in WebStorm and other JetBrains IDEs you need to install [this plugin][jb-plugin].

[jb-plugin]: https://plugins.jetbrains.com/plugin/8578-@hishprorg/nam-inventore

## Security Contact

To report a security vulnerability, please use the [Tidelift security contact].
Tidelift will coordinate the fix and disclosure.

[Tidelift security contact]: https://tidelift.com/security


## For Enterprise

Available as part of the Tidelift Subscription.

The maintainers of `@hishprorg/nam-inventore` and thousands of other packages are working
with Tidelift to deliver commercial support and maintenance for the open source
dependencies you use to build your applications. Save time, reduce risk,
and improve code health, while paying the maintainers of the exact dependencies
you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-@hishprorg/nam-inventore?utm_source=npm-@hishprorg/nam-inventore&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
