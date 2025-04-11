# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.0.2.1] - 2025-04-11

### Changed

- requiring `rqrcode_core`

## [3.0.2] - 2025-04-11

### Added

### Changed

- using forked version of `rqrcode_core` to `1.2.0` since the main gem still uses rexml

### Breaking Change

## [3.0.1] - 2025-04-10

### Added

### Changed

- minor bump `rqrcode_core` to `1.2.0`

### Breaking Change

## [3.0.0] - 2025-04-10

### Added

### Changed

- README updated
- patch bump `ast` to `2.4.3`
- minor bump `json` to `2.10.2`
- patch bump `language_server-protocol` to `3.17.0.4`
- patch bump `parser` to `3.3.7.4`
- add `prism-1.4.0`
- remove `rexml`
- minor bump `regexp_parser` to `2.10.0`
- minor bump `stardard` to `1.49.0`

### Breaking Change


## [2.2.0] - 2023-06-17

### Changed

* Allow all ChunkyPNG::Color options to be passed into `fill` and `color` on `as_png` [#135]
* Add 3.2 to CI [@petergoldstein](https://github.com/petergoldstein) [#133]
* Development dependency upgrades. Minimum Ruby change [#130]
* README updates

## [2.1.2] - 2022-07-26

### Changed

* Remove setup script as it just calls bundle install [#128]
* Change inline styles to the fill property to allow for strict CSP style-src directive [#127]

## [2.1.1] - 2022-02-11

### Added

- Added in a handler for when color arguments are passed in as symbols e.g `color: :yellow`. This also allows for the use of the `:currentColor` keyword. [#122]

## [2.1.0] - 2021-08-26

### Changed

- Sync Gemfile.lock with `rqrcode_core.1.2.0` [Adds Multimode Support](https://github.com/whomwah/rqrcode_core#multiple-encoding-support)

### Added

- Add badge for Standard linting

### Changed

- Corrected method name referred to in CHANGELOG.

## [2.0.0] - 2021-05-06

### Added

- A new `use_path:` option on `.as_svg`. This uses a `<path>` node to greatly reduce the final SVG size. [#108]
- A new `viewbox:` option on `.as_svg`. Replaces the `svg.width` and `svg.height` attribute with `svg.viewBox` to allow CSS scaling. [#112]
- A new `svg_attributes:` option on `.as_svg`. Allows you to pass in custom SVG attributes to be used in the `<svg>` tag. [#113]

### Changed

- README updated
- Rakefile cleaned up. You can now just run `rake` which will run specs and fix linting using `standardrb`
- Small documentation clarification [@smnscp](https://github.com/smnscp)
- Bump `rqrcode_core` to `~> 1.0`

### Breaking Change

- The dependency `rqrcode_core-1.0.0` has a tiny breaking change to the `to_s` public method. https://github.com/whomwah/rqrcode_core/blob/master/CHANGELOG.md#breaking-changes

## [1.2.0] - 2020-12-26

### Changed

- README updated
- bump dependencies
- fix `required_ruby_version` for Ruby 3 support

[unreleased]: https://github.com/whomwah/rqrcode/compare/v2.2.0...HEAD
[2.2.0]: https://github.com/whomwah/rqrcode/compare/v2.1.2...v2.2.0
[2.1.2]: https://github.com/whomwah/rqrcode/compare/v2.1.1...v2.1.2
[2.1.1]: https://github.com/whomwah/rqrcode/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/whomwah/rqrcode/compare/v2.0.0...v2.1.0
[2.0.0]: https://github.com/whomwah/rqrcode/compare/v1.2.0...v2.0.0
[1.2.0]: https://github.com/whomwah/rqrcode/compare/v1.1.1...v1.2.0
