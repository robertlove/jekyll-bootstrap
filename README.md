# Jekyll/Bootstrap

![Jekyll](https://img.shields.io/badge/jekyll-v3.8.5-3F1F1F.svg)
![Bootstrap](https://img.shields.io/badge/bootstrap-v4.3.1-563d7c.svg)
![jQuery](https://img.shields.io/badge/jquery-v3.4.1-0769ad.svg)
![Popper.js](https://img.shields.io/badge/popper-v1.15.0-21b2a6.svg)

Jekyll/Bootstrap is a Jekyll starter project for GitHub Pages with Bootstrap baked right in.

[Jekyll](https://jekyllrb.com/) is a static website generator that works seamlessly with [GitHub Pages](https://pages.github.com/). Whilst [Bootstrap](https://getbootstrap.com/) is the world's most popular front-end component library. Put this all together and you get a fast, secure and highly customisable static website with free hosting.

Jekyll/Bootstrap solves the confusing task of integrating Bootstrap with Jekyll by doing the integration for you - *the right way* - then guiding you through the simple process of customising Bootstrap - *the right way*.

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

The first thing you'll want to do is open [`_config.yml`](_config.yml) and update the `title`, `description`, `baseurl` and `url` configuration options. Remember that configuration changes require you to rerun `$ bundle exec jekyll serve` in order for the changes to take effect.

For a full list of configuration options, see [Jekyll Configuration](https://jekyllrb.com/docs/configuration/).

### Customising Bootstrap

One of the biggest criticisms of Bootstrap is that it makes your website look like every other Bootstrap website out there. This criticism is borne out of ignorance. Used properly, you'll be able to customise Bootstrap to make even the pickiest designer proud of you.

The process is:

1. Use Bootstrap components and classes in your HTML - there are many (and many utility classes are undocumented)
1. Override and extend Bootstrap's default variables in [`_sass/_variables.scss`](_sass/_variables.scss)
1. Write custom styles in [`assets/css/style.css`](assets/css/style.scss)

Done correctly, you'll likely never get to step 3. If you do get to step 3, before continuing, have another think about the way you're architecting your front-end.

For a full list of variables, see [Bootstrap SCSS Variables](https://github.com/twbs/bootstrap/blob/master/scss/_variables.scss).

## Contributing

See [Contributing](https://github.com/robertlove/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/robertlove/jekyll-bootstrap/graphs/contributors).

## License

See [LICENSE](LICENSE).
