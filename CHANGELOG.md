# changelog

[![Keep a Changelog](https://img.shields.io/badge/Keep%20a%20Changelog-1.0.0-informational)](https://keepachangelog.com/en/1.0.0/)
[![Semantic Versioning](https://img.shields.io/badge/Sematic%20Versioning-2.0.0-informational)](https://semver.org/spec/v2.0.0.html)
![clq validated](https://img.shields.io/badge/clq-validated-success)

Keep the newest entry at top, format date according to ISO 8601: `YYYY-MM-DD`.

Categories, defined in [changemap.json](.github/clq/changemap.json):

- *major* release trigger:
  - `Changed` for changes in existing functionality.
  - `Removed` for now removed features.
- *minor* release trigger:
  - `Added` for new features.
  - `Deprecated` for soon-to-be removed features.
- *bugfix* release trigger:
  - `Fixed` for any bugfixes.
  - `Security` in case of vulnerabilities.

## [1.0.3] - 2025-03-04

### Fixed

- The untag script was not closing the if statement
- Use the tag comment to map a tag to a workflow run

## [1.0.2] - 2025-03-04

### Fixed

- Previous refactoring lost a space

## [1.0.1] - 2025-03-04

### Fixed

- Git requires a message when tagging
- Bad multi-line test in bash

## [1.0.0] - 2025-03-04

### Added

- Extracted from common-module
