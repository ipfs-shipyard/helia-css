# @helia/css <!-- omit in toc -->

> 🍴 Forked from https://github.com/ipfs-shipyard/ipfs-css

The single-purpose CSS class names and @font-face config to Helia up your UI.

Pairs well with [tachyons].

## Table of contents <!-- omit in toc -->

- [Install](#install)
- [Usage](#usage)
  - [CSS in JS](#css-in-js)
  - [Less](#less)
  - [SCSS](#scss)
- [Icons](#icons)
- [Colors](#colors)
- [License](#license)
- [Contribute](#contribute)

## Install

Add `@helia/css` to your project via npm:

```sh
npm install @helia/css
```

## Usage

Once you've installed `@helia/css` from npm, the CSS and SCSS files and the web-fonts are available from your `node_modules/@helia/css` directory.

If you are set up with a build process that lets you import css files directly from `node_modules`, then you can just add the following to your CSS file.

```css
@import 'tachyons'; /* Optional, jolly good tho */
@import '@helia/css';
```

The file includes font-face definitions and single purpose CSS class names that you can compose freely, to create your lovely UI.

```html
<header class='pa2 bg-navy'>
  <h2 class='ma0 montserrat aqua'>
    OH HAI! It's so nice to see you again.
  </h2>
</header>
```

### CSS in JS

You can import the `theme.json` file which can be used with a [ThemeProvider] component.

All **the CSS atoms are generated** from that, so you can be sure you're using the same values.

### Less

`helia.css` is a regular CSS file, so you can import it normally. Each declaration has a single purpose, so if you prefer to compose your rules outside the DOM, you can safely use them as mixins:

```less
.my-lovely-widget {
  .aqua;
  .bg-navy;
  .montserrat;
}
```

### SCSS

While `helia.css` contains everything you need, if you prefer variables for fonts, colors and gradients, these are there for you in `theme.scss`.

## Icons

See: https://dweb.link/ipfs/bafybeiebays3i7aem7tptga3kilzux7f5gz6czl4dietazgutcjhozjviu

## Colors

<img title='#073a53' src='https://swatch.now.sh?color=%23073a53&name=navy' /><img title='#244e66' src='https://swatch.now.sh?color=%23244e66&name=navy-muted' /><img title='#69c4cd' src='https://swatch.now.sh?color=%2369c4cd&name=aqua' /><img title='#9ad4db' src='https://swatch.now.sh?color=%239ad4db&name=aqua-muted' />

<img title='#b7bbc8' src='https://swatch.now.sh?color=%23b7bbc8&name=gray' /><img title='#d9dbe2' src='https://swatch.now.sh?color=%23d9dbe2&name=gray-muted' /><img title='#34373f' src='https://swatch.now.sh?color=%2334373f&name=charcoal' /><img title='#7f8491' src='https://swatch.now.sh?color=%237f8491&name=charcoal-muted' />

<img title='#ea5037' src='https://swatch.now.sh?color=%23ea5037&name=red' /><img title='#f36149' src='https://swatch.now.sh?color=%23f36149&name=red-muted' /><img title='#f7df1e' src='https://swatch.now.sh?color=%23f7df1e&name=yellow' /><img title='#f9a13e' src='https://swatch.now.sh?color=%23f9a13e&name=yellow-muted' />

<img title='#378085' src='https://swatch.now.sh?color=%23378085&name=teal' /><img title='#439a9d' src='https://swatch.now.sh?color=%23439a9d&name=teal-muted' /><img title='#0cb892' src='https://swatch.now.sh?color=%230cb892&name=green' /><img title='#0aca9f' src='https://swatch.now.sh?color=%230aca9f&name=green-muted' />

<img title='#f3f4f7' src='https://swatch.now.sh?color=%23f3f4f7&name=snow' /><img title='#f7f8fa' src='https://swatch.now.sh?color=%23f7f8fa&name=snow-muted' /><img title='#117eb3' src='https://swatch.now.sh?color=%23117eb3&name=link' />

## License

Licensed under either of

- Apache 2.0, ([LICENSE-APACHE](LICENSE-APACHE) / <http://www.apache.org/licenses/LICENSE-2.0>)
- MIT ([LICENSE-MIT](LICENSE-MIT) / <http://opensource.org/licenses/MIT>)

## Contribute

Contributions welcome! Please check out [the issues](https://github.com/ipfs/js-ipfs-unixfs/issues).

Also see our [contributing document](https://github.com/ipfs/community/blob/master/CONTRIBUTING_JS.md) for more information on how we work, and about contributing in general.

Please be aware that all interactions related to this repo are subject to the IPFS [Code of Conduct](https://github.com/ipfs/community/blob/master/code-of-conduct.md).

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.

[![](https://cdn.rawgit.com/jbenet/contribute-ipfs-gif/master/img/contribute.gif)](https://github.com/ipfs/community/blob/master/CONTRIBUTING.md)

[ipfs.io]: https://ipfs.io
[tachyons]: http://tachyons.io
[CC-BY-SA 3.0]: https://ipfs.io/ipfs/QmVreNvKsQmQZ83T86cWSjPu2vR3yZHGPm5jnxFuunEB9u
[ThemeProvider]: https://glamorous.rocks/advanced/#theming
