# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- `redstoneSide` config option can now be a table, if you wish to have multiple outputs for redstone heartbeat

## 1.0.1
### Fixed
- Fixed broken error handler

## 1.0.0
### Added
- Major version mismatch safety warning
- Predicate system for more specific item matching

### Fixed
- Fixed compatibility for multiple items with the same modid

### Changed
- Tables **must** have class 'stock-table' to be filled with stock data
- Instead of putting the modid as the key in the `items` table in the config, you **must** now use numerical keys (don't use explicit keys), and instead put the modid as a config option. For example:
```
items = {
  {
    modid = "minecraft:glowstone",
    disp  = "Glowstone Block",
    addy  = "glow",
    price = 3
  }
}
```

## 0.0.7 - 2018-05-20
### Added
- Added sanity checks for peripheral wraps

### Fixed
- Discord webhooks now work

### Changed
- Updated examples

## 0.0.6 - 2018-05-20
### Fixed
- Fixed a bug with message templates

### Changed
- Error message for invalid config is cleaner

## 0.0.5 - 2018-05-20
### Fixed
- Fixed a bug in vendor libraries, preventing transactions going through when checkForUpdates is enabled

## 0.0.4 - 2018-05-19
### Fixed
- Fixed fatal crash due to missing lib functions

## 0.0.3 - 2018-05-19
### Fixed
- Update notifications work properly

## 0.0.2 - 2018-05-19
### Changed
- New version checking is now done asyncronously

### Fixed
- Fix redstone/inventory intervals being longer than configured
- `line-height` property now works correctly

## 0.0.1 - 2018-05-19
### Added
- This CHANGELOG file
- The release of Xenon