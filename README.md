# Jekyll/Bootstrap

![Jekyll](https://img.shields.io/badge/Jekyll-v3.9.0-red.svg)
![Bootstrap](https://img.shields.io/badge/Bootstrap-v5.0.0--beta1-blueviolet)
![Bootstrap Icons](https://img.shields.io/badge/Bootstrap%20Icons-v1.2.0-blueviolet)

Jekyll/Bootstrap is a Jekyll starter project for GitHub Pages with Bootstrap baked right in.

Jekyll/Bootstrap solves the confusing task of integrating Bootstrap with Jekyll by doing the integration for you - *the right way* - then guiding you through the simple process of customising Bootstrap - *the right way*.

[Jekyll](https://jekyllrb.com/) is a static website generator that works seamlessly with [GitHub Pages](https://pages.github.com/). Whilst [Bootstrap](https://getbootstrap.com/) is the world's most popular front-end component library. Put this all together and you get a fast, secure and highly customisable static website with free hosting.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Installation

Before you begin, ensure you've installed [Jekyll](https://jekyllrb.com/). Then:

1. `$ git clone https://github.com/robertlove/jekyll-bootstrap.git`
1. `$ cd jekyll-bootstrap`
1. `$ bundle install`
1. `$ bundle exec jekyll serve`

If all went well, you'll be able to view your new Jekyll/Bootstrap website locally by going to http://127.0.0.1:4000/jekyll-bootstrap/ in your browser.

## Usage

### Configuration

- Open [`_config.yml`](_config.yml) and update the following configuration options:
  - `title`
  - `description`
  - `baseurl`
  - `url`
  - `twitter`
- Replace `/favicon.ico` with your own favicon
- Replace `/assets/img/image.jpg` with your own image

**Note:** Changes to `_config.yml` require you to rerun `$ bundle exec jekyll serve` in order for the changes to take effect.

For a full list of configuration options, see [Jekyll Configuration](https://jekyllrb.com/docs/configuration/).

### Customising Bootstrap

One of the biggest criticisms of Bootstrap is that it makes your website look like every other Bootstrap website out there. This criticism is borne out of ignorance. Used properly, you'll be able to customise Bootstrap to make even the pickiest designer proud of you.

The process is:

1. Use Bootstrap components and classes in your HTML - there are many (and many utility classes are undocumented)
1. Override Bootstrap's default variables in [`_sass/_variables.scss`](_sass/_variables.scss)
1. Write custom styles in [`assets/css/style.css`](assets/css/style.scss)
1. Write custom scripts in [`assets/js/script.js`](assets/js/script.js)

For a full list of classes - including the undocumented ones, see [Bootstrap CSS](https://github.com/twbs/bootstrap/blob/master/dist/css/bootstrap.css)

For a full list of variables, see [Bootstrap SCSS Variables](https://github.com/twbs/bootstrap/blob/master/scss/_variables.scss).

**Note:** Done correctly, you'll likely never get to steps 3 and 4. If you do, before continuing, have another think about the way you're architecting your front-end.

### Icons

Jekyll/Bootstrap comes with [Bootstrap Icons](https://icons.getbootstrap.com/) pre-installed. Use the icon include for all your icon needs. The `name` parameter is used to specify the icon and is required. The `class` parameter is used to add any additional classes for styling and is optional.

```
{% include icon.html name='github' class='text-danger' %}
```

### Using Third-party Libraries

Sometimes you'll want to use third-party libraries to achieve the results you're after. For example, you might want to use [Prism](https://prismjs.com/) for syntax highlighting or [Moment.js](https://momentjs.com/) for displaying dates and times in JavaScript.

To use a third-party library:

#### Styles

1. Copy any `*.css` or `*.scss` files to the [`_sass`](_sass) folder
1. Rename any `*.css` files to `*.scss` (e.g. rename `prism.css` to `prism.scss`)
1. Open [`assets/css/style.css`](assets/css/style.scss) and import your SCSS file(s) (e.g. `@import "path/to/prism";` - leaving out the `.scss` file extension)

This will compile and minify all styles into `_site/assets/css/style.css`.

#### Scripts

1. Copy any `*.js` files to the [`assets/js`](assets/js) folder
1. Open [`assets/js/script.js`](assets/js/script.js) and import your JavaScript file(s) (e.g. `{% include_relative path/to/prism.js %}`)
1. Open [`_config.yml`](_config.yml) and add your JavaScript file(s) to the list of excludes under `exclude:` (e.g. `  - assets/js/path/to/prism.js`)

This will compile (but not minify) all scripts into `_site/assets/js/script.js`. Jekyll doesn't support minification of JavaScript files on GitHub Pages. If you want your scripts to be minified, use the minified versions supplied by the third-party library.

## Contributing

See [Contributing](https://github.com/robertlove/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/robertlove/jekyll-bootstrap/graphs/contributors).

## License

See [LICENSE](LICENSE).
