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

## [1.2.0] - 2025-04-18

### Added

- When the gradle build fails, attach all the reports to the
  [worhflow artifacts](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/storing-and-sharing-data-from-a-workflow)

## [1.1.0] - 2025-03-31

### Added

- Reads the JVM version and vendor from the gradle daemon configuration, defaulting to `corretto 21`.
- Emits the module name. By convention, the module name of a gradle module is the name of the root project, which should also be the repository name

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
