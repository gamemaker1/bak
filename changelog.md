# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased](https://github.com/gamemaker1/bak/tree/main)

## [0.2.0](https://github.com/gamemaker1/bak/releases/tag/0.2.0) - 05 August 2021

### Changed

- Convert .txt files to .md files
- Add a release note generation step to the release workflow (See #1)
- Move `-s` option from `scripts/dist` to `.fpm` to avoid repitition.

### Added

- Allow for skipping checksum generation using the `-C none` option.

## [0.1.1](https://github.com/gamemaker1/bak/releases/tag/0.1.1) - 03 August 2021

### Fixes

- Fixed bug where tar used to error out when using tar-gz compression format.

## [0.1.0](https://github.com/gamemaker1/bak/releases/tag/0.1.0) - 01 August 2021

### Added

- The -c, -C, -f, -d and -e flags.
- Creating archives using tar (gzip, xz, zstd, bzip2) and zip.
- Computing checksums of all files inside the archive using md5, sha1, sha224, sha384, sha256, sha512 and b2.
- Binary packages contain the manpage and license along with the program.
- Binary packages are built for Debian, RedHat, Arch Linux, Alpine Linux, Snap, FreeBSD, and MacOS, along with a generic tarball.
