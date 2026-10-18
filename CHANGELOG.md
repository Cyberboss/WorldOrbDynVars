# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/2.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

# [2.0.1] - 2026-10-18

### Fixed

- Fixed `DynamicVariableSpace` also being created next to `UserRoot` components. (@Cyberboss)

## [2.0.0] - 2026-10-18

### Changed

- **Breaking:** The `DynamicVariableSpace` now only allows direct binding. (@Cyberboss)
- Modernized code and CI. (@Cyberboss)

# [1.1.1] - 2026-08-27

### Fixed

- Update latest reference assemblies to fix errors. (@Cyberboss)

# [1.1.0] - 2026-08-27

### Added

- Added `SessionUrlsReference` variable to the `SyncFieldList<Uri>` for `ActiveSessionURLs`. (@Cyberboss)

# [1.0.2] - 2026-05-15

### Changed

- Build against reference assemblies. (@Cyberboss)

# [1.0.1]

### Added

- Log the parent slot ref instead of name as it's not set to a meaningful value when `WorldOrb` components are started. (@Cyberboss)

### Fixed

- Fixed `NullReferenceException` due to `null` locale `messages`. (@Cyberboss)
- Fixed attempting to run in local home where there is no local user to reference for naming the child slot. (@Cyberboss)

# [1.0.0]

### Added

- Initial release. (@Cyberboss)

[2.0.1]: https://github.com/Cyberboss/WorldOrbDynVars/tree/v2.0.0...v2.0.1
[2.0.0]: https://github.com/Cyberboss/WorldOrbDynVars/tree/v1.1.1...v2.0.0
[1.1.1]: https://github.com/Cyberboss/WorldOrbDynVars/tree/v1.1.0...v1.1.1
[1.0.0]: https://github.com/Cyberboss/WorldOrbDynVars/tree/v1.0.0
