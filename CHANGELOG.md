# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Fixed

- The `helm.sh/chart` label is valid for long chart versions: the 63-character cut trims the whole trailing run of `-`, `.` and `_`.

### Changed

- CI: architect orb 10.16.7, which pushes the chart to the git catalog with the architect GitHub App instead of the `catalogbot` account. A pre-release tag (`v1.2.3-rc.1`) now goes to the test catalog only, and the published chart version is posted as a pull request comment.
- Migrate Chart.yaml annotations to new format as per https://docs.giantswarm.io/reference/platform-api/chart-metadata/

## [1.0.1] - 2025-09-16

### Removed

- Remove `attributeRestrictions` from RBAC manifest

## [1.0.0] - 2024-11-06

### Changed

- Migrated build system to `app-build-suite`.
  - Made the app compliant with ABS imposed static rules.

### Added

- Added network policy support.

### Removed

- Removed PSP support.

## [0.1.2] - 2020-07-30

### Updated

- Add release automation.

## [0.1.1] - 2020-03-17

### Updated

- Increment version for testing updates.

## [0.1.0] - 2020-03-17

### Added

- Add initial version.

[Unreleased]: https://github.com/giantswarm/test-app/compare/v1.0.1...HEAD
[1.0.1]: https://github.com/giantswarm/test-app/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/giantswarm/test-app/compare/v0.1.2...v1.0.0
[0.1.2]: https://github.com/giantswarm/test-app/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/giantswarm/test-app/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/giantswarm/test-app/releases/tag/v0.1.0
