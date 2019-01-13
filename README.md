# sublime-icon-fonts

[![The MIT License](https://img.shields.io/badge/license-MIT-orange.svg?style=flat-square)](http://opensource.org/licenses/MIT)
[![Package Control](https://packagecontrol.herokuapp.com/downloads/Icon%20Fonts.svg?style=flat-square)](https://packagecontrol.io/packages/Icon%20Fonts)
[![GitHub release](https://img.shields.io/github/release/idleberg/sublime-icon-fonts.svg?style=flat-square)](https://github.com/idleberg/sublime-icon-fonts/releases)
[![CircleCI](https://flat.badgen.net/circleci/github/idleberg/sublime-icon-fonts)](https://circleci.com/gh/idleberg/sublime-icon-fonts/)

**Note:** *As of v6.1, this package supports all __Font Awesome v5__ icons. If you need to continue the old __Font Awesome v4__ icons, please install the [“Icon Fonts (Legacy)”](https://packagecontrol.io/packages/Icon%20Fonts%20%28Legacy%29) package via Package Control!*

Sublime Text snippets for several popular icon fonts ([see details](https://github.com/idleberg/sublime-icon-fonts#prefixes)).

This package is also available for [Atom](https://github.com/idleberg/atom-icon-fonts) and [Visual Studio Code](https://github.com/idleberg/vscode-icon-fonts).

![Screenshot](https://raw.github.com/idleberg/sublime-icon-fonts/master/screenshot.gif)

*Screenshot using the [Hopscotch](https://github.com/idleberg/Hopscotch) color scheme*

## Installation

### Package Control

1. Make sure you already have [Package Control](https://packagecontrol.io/) installed
2. Choose *“Install Package”* from the Command Palette (<kbd>Super</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>)
3. Select *“Icon Fonts”* and press <kbd>Enter</kbd>

### GitHub

1. Change to your Sublime Text `Packages` directory
2. Clone repository `git clone https://github.com/idleberg/sublime-icon-fonts "Icon Fonts"`

## Usage

Snippets are limited to the `html` and `css|less|sass|scss|stylus` scopes, which might not be activated in your `auto_complete_selector` user preferences by default. However, you can still force the completion popup to show by pressing <kbd>Ctrl</kbd>+<kbd>Space</kbd>.

Typing the class name of an icon using the designated prefix will complete to a tag containing the icon class. Exceptions are `fa-layers`, `fa-layers-counter`, `fa-layers-text` and `fa-layers` (`<span>`).

### Prefixes

Prefix            | Icon Font                           | Version | cdnjs | jsDelivr
------------------|-------------------------------------|---------|-------|---------
`ai`              | [Android Icons][ai]                 | 1.0.0   | 🚫    | 🚫
`brandico`        | [Brandico Font][brandico]           | –       | 🚫    | 🚫
`cc`              | [Creative Commons Icon Font][cc]    | 1.2.1   | ✅    | ✅
`dashicons`       | [WordPress Dashicons][dashicons]    | –       | 🚫    | 🚫
`devicons`        | [Devicons][devicons]                | 1.8.0   | ✅    | ✅
`el`              | [Elusive Icons][el]                 | 2.0.0   | 🚫    | 🚫
`fas`,`far`,`fab` | [Font Awesome Pro][fa]              | 5.0.0   | ✅    | ✅
`fi`              | [Foundation Icons][fi]              | 3.0     | ✅    | ✅
`fl`              | [Font Linux][fl]                    | 0.9     | 🚫    | 🚫
`geomicon`        | [Geomicons Open][geomicon]          | 2.0.0   | 🚫    | ✅
`glyphicon`       | [Bootstrap Glyphicons][glyphicon]   | 3.3.6   | 🚫    | 🚫
`icofont`         | [ShapeBootstrap IcoFont][icofont]   | 1.0.0b  | 🚫    | 🚫
`icono`           | [Icono][icono]                      | 1.3.0   | ✅    | 🚫
`ion`             | [Ionicons][ion]                     | 2.0.1   | 🚫    | 🚫
`mdi`             | [Material Design Icons][mdi]        | 1.7.22  | ✅    | 🚫
`mfg`             | [MFG Labs Iconset][mfg]             | –       | 🚫    | 🚫
`mfizz`           | [Font Mfizz][mfizz]                 | 2.3.0   | ✅    | 🚫
`octicon`         | [GitHub Octicons][octicon]          | 4.1.0   | 🚫    | 🚫
`oi`              | [Open Iconic][oi]                   | 1.1.0   | 🚫    | ✅
`openwebicons`    | [OpenWeb Icons][openwebicons]       | 1.4.3   | ✅    | ✅
`pf`              | [PaymentFont][pf]                   | 1.1.2   | ✅    | 🚫
`ratchicon`       | [Ratchicons][ratchicon]             | 2.0.2   | ✅    | ✅
`st`              | [Stack Icons][st]                   | 1.0.0   | 🚫    | 🚫
`typcn`           | [Typicons][typcn]                   | 2.0.7   | 🚫    | 🚫
`ui`              | [Semantic UI Icons][ui]             | 2.0.7   | ✅    | ✅
`wi`              | [Weather Icons][wi]                 | 2.0.10  | ✅    | 🚫
`zmdi`            | [Material Design Iconic Font][zmdi] | 2.2.0   | ✅    | 🚫

Several previously supported fonts have been removed and are now available in the [SVG Icon Snippets](https://github.com/idleberg/sublime-svg-icons) package or the icon fonts [legacy package](https://github.com/idleberg/sublime-icon-fonts-legacy).

**Examples**:

* `fa-check`+<kbd>Tab</kbd> completes to `<i class="fa fa-check"></i>`
* `glyphicon-check`+<kbd>Tab</kbd> completes to `<span class="glyphicon glyphicons-check"></span>`
* well, you get the idea

Snippets also work in the `text.css` scope, where they complete to the Unicode value of an icon.

**Example**:

* `fa-check`+<kbd>Tab</kbd> completes to `'\f00c'`

These snippets also work for Less, SCSS and Stylus files!

### CDNs

If a supported CDN is indicated in the [table](#prefixes) above, you can use the prefixes `cdnjs`, `jsdelivr`, `maxcdn` to quickly insert a link to the CDN-hosted asset:

Examples:

* `cdnjs-fa`+<kbd>Tab</kbd> completes to a `<link>` tag to the Font Awesome style-sheet
* `jsdelivr-fa`+<kbd>Tab</kbd> completes to a `<link>` tag to the Font Awesome style-sheet
* `jsdelivr-geomicon`+<kbd>Tab</kbd> completes to a `<script>` tag to the Geomicons script
* `maxcdn-fa`+<kbd>Tab</kbd> completes to a `<link>` tag to the Font Awesome style-sheet

## License

This work is licensed under the [The MIT License](LICENSE).

## Donate

You are welcome support this project using [Flattr](https://flattr.com/submit/auto?user_id=idleberg&url=https://github.com/idleberg/sublime-icon-fonts) or Bitcoin `17CXJuPsmhuTzFV2k4RKYwpEHVjskJktRd`

[ai]: http://www.androidicons.com
[brandico]: https://github.com/fontello/brandico.font
[cc]: https://github.com/cc-icons/cc-icons
[dashicons]: https://github.com/WordPress/dashicons
[devicons]: https://github.com/vorillaz/devicons
[el]: https://github.com/reduxframework/Elusive-Icons
[fa]: https://github.com/FortAwesome/Font-Awesome
[fi]: http://zurb.com/playground/foundation-icons
[fl]: https://github.com/Lukas-W/font-linux
[geomicon]: https://github.com/jxnblk/geomicons-open
[glyphicon]: https://getbootstrap.com/components/#glyphicons
[icofont]: http://icofont.com/
[icono]: https://github.com/saeedalipoor/icono
[ion]: https://github.com/driftyco/ionicons
[line]: http://www.elegantthemes.com/blog/resources/how-to-use-and-embed-an-icon-font-on-your-website
[mdi]: https://github.com/Templarian/MaterialDesign-Webfont
[mfg]: https://github.com/MfgLabs/mfglabs-iconset
[mfizz]: https://github.com/fizzed/font-mfizz
[octicon]: https://github.com/primer/octicons/tree/v4.1.0
[oi]: https://github.com/iconic/open-iconic
[openwebicons]: https://github.com/pfefferle/openwebicons
[pf]: https://github.com/vendocrat/PaymentFont
[ratchicon]: http://goratchet.com/components/#ratchicons
[st]: https://github.com/parkerbennett/stackicons
[typcn]: https://github.com/stephenhutchings/typicons.font
[ui]: http://semantic-ui.com/elements/icon.html
[wi]: https://github.com/erikflowers/weather-icons
[zmdi]: https://github.com/zavoloklom/material-design-iconic-font
