# Changelog

## 1.1.12 - 2021-11-01

### Fixed
- Fix JS Redactor plugin not installing correctly in some instances.

## 1.1.11 - 2021-09-07

### Fixed
- Fix Icons Path plugin setting not working correctly when using aliases.

## 1.1.10 - 2020-12-07

### Changed
- Update Font Awesome remote source to 5.15.1.

### Fixed
- Ensure icons load in Super Table and other nesting fields.

## 1.1.9 - 2020-08-11

### Added
- Allow `iconSetsPath` settings to use environment variables or aliases.
- Allow `iconSetsUrl` settings to use environment variables or aliases.

## 1.1.8 - 2020-06-10

### Added
- Added `iconPickerField.length` and `iconPickerField.getLength()`.
- Added `iconPickerField.isEmpty` and `iconPickerField.getIsEmpty()`.

## 1.1.7 - 2020-06-09

### Fixed
- Fix error when only a single sprite existed in a sprite sheet.

## 1.1.6 - 2020-06-08

### Fixed
- Improve performance of remote icon sets. (thanks @bertoost).

## 1.1.5 - 2020-06-06

### Added
- Add `enableCache` setting.

### Fixed
- Fix `entry.iconField` direct output showing URL, even when an icon isn’t picked.

## 1.1.4 - 2020-04-16

### Fixed
- Fix logging error `Call to undefined method setFileLogging()`.

## 1.1.3 - 2020-04-15

### Changed
- File logging now checks if the overall Craft app uses file logging.
- Log files now only include `GET` and `POST` additional variables.

## 1.1.2 - 2020-02-11

### Fixed
- Fix windows path issues.
- Fix another potential error for field settings and icon sets.

## 1.1.1 - 2020-01-12

### Fixed
- Fix error with remote sets set to “All”.
- Fix error when installing for the first time.

## 1.1.0 - 2020-01-12

### Added
- Add GraphQL support for field. Now returns an IconModel.
- Add cache for each icon set. Icons for each set are now cached when the Icon Picker field is saved.
- Add controller action to lazy-load icon set content.
- Add utility to re-generate icon set caches.
- Improve performance for large icon sets.
- Add Redactor support. See [docs](https://verbb.io/craft-plugins/icon-picker/docs/feature-tour/redactor).
- Add support for [Google Material Design Icons](https://github.com/google/material-design-icons), which need some special-handling.

### Changed
- Major refactor, bringing performance improvements and caching.
- Update the icon selection field to lazy-load icons, rather than loading on page load. This brings significant performance benefits

### Fixed
- Fix `craft.iconPicker.spritesheet` not always returning content.

## 1.0.10 - 2019-09-04

### Fixed
- Fix numerous errors when fetching remote icon sets via URL.
- Change Font Awesome icon source to use file-system fetching, rather than via HTTP.

## 1.0.9 - 2019-09-03

### Fixed
- Fix icons not propagating to other sites.

## 1.0.8 - 2019-08-17

### Added
- Add `getPath()` function to icon model.
- Add supported translation methods for field.

### Changed
- Changing to Local file read from External URL.

### Fixed
- Fix error when resolving font awesome json file path.
- Fix error when trying to access remote icons sets.
- Fix error with font-name for icon font files.

## 1.0.7 - 2019-04-27

### Fixed
- Fix Live Preview not showing icon selection.
- Fix Neo fields clipping icon selection.
- Icon selection pane now attaches itself to the field, instead of the body.

## 1.0.6 - 2019-04-24

### Added
- Add `maxIconsShown` to control how many icons should be shown in the selection pane.

### Changed
- Update default `iconSetsPath` to be relative to the web folder - `CRAFT_BASE_PATH . '/web/icons/'`.

### Fixed
- Fix compatibility with some sprite definitions.
- Fix handling when no sub-folders in icon path, only single icons.

## 1.0.5 - 2019-04-07

### Added
- Add `model.hasIcon()`.

### Fixed
- Fix normalise-url function causing issues in some cases.

## 1.0.4 - 2019-03-17

### Added
- Add settings override notices for plugin settings screen.

### Fixed
- Fix SSL errors with spritesheets and icon sources when devMode is on.

## 1.0.3 - 2019-03-07

### Fixed
- Fix overflow issue for some fields.

## 1.0.2 - 2019-03-06

### Fixed
- Fix JS error causing issues across the control panel.

## 1.0.1 - 2019-03-05

- Initial (full) release.

## 1.0.0 - 2019-01-28

- Initial (beta) release.
