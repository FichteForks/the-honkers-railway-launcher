# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.2.0] - 24.05.2023

### Added

- Added Italian
- Added Indonesian
- Added dynamic main button icon switching
- Set button label as "Resume" when the diff is part downloaded
- Added options to use wine / gstreamer shared libraries from selected wine build.
  These options will configure `LD_LIBRARY_PATH` and `GST_PLUGIN_PATH` environment variables
- Added setting of `LC_ALL` in wine lang setting
- Added `LAUNCHER_REQUESTS_TIMEOUT` environment variable
- Added option to disable main patch applying

### Fixed

- Fixed session applying on each launcher start
- Fixed predownload button ui
- Fixed proton builds integration with sandbox
- Fixed compatibility between sessions manager and sandbox
- Fixed sandboxing of inexisting folders

### Changed

- Apply selected session before launching the game.
  This will properly save your game session when you switch between wine prefixes
- Redesigned main button
- Used `whatadistro` to identify recommended package manager in the first run window
- Moved a lot of settings to separate page
- Set fsr quality mode in enhancements settings instead of strength
- Updated fps unlocker data
- Made temporary workaround to the game API changes
- Increased default requests timeout to 8 seconds
- Updated minreq to support `http_proxy`-like variables
- Disabled xlua patch applying by default

### Removed

- Removed Futex2 wine sync option

## [1.1.0] - 06.05.2023

### Added

- Added game settings section
- Added game sessions manager
- Added `LAUNCHER_FOLDER` variable support.
  Using this you can specify root path where the launcher stores `config.json` and other files
- Added patch repository mirror

### Changed

- Improved launcher logo rendering quality
- Reworked entry rows in the settings

### Fixed

- Fixed sandboxed game running (sounds are broken for now)

## [1.0.0] - 01.05.2023

🚀 Initial release

<br>

[unreleased]: https://github.com/an-anime-team/the-honkers-railway-launcher/compare/1.2.0...next
[1.2.0]: https://github.com/an-anime-team/the-honkers-railway-launcher/compare/1.1.0...1.2.0
[1.1.0]: https://github.com/an-anime-team/the-honkers-railway-launcher/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/an-anime-team/the-honkers-railway-launcher/releases/tag/1.0.0
