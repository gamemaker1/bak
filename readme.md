# bak 0.1.1

A backup tool (written in bash)

## Installation

The latest releases for various platforms can be found [here](https://github.com/gamemaker1/bak/releases/latest).

- Debian - .DEB
- RedHat - .RPM
- Arch Linux - .pkg.tar.zst [Also on AUR as bak, bak-bin or bak-git]
- Alpine Linux - .apk
- Snap - .snap
- FreeBSD - .freebsd
- MacOS - .pkg
- Generic - .tar.gz

Manual installation can be done by downloading and extracting the files from
the `Generic` release. Here is where to put the files from the archive:

- source/bak => /usr/bin/bak
- man/bak.1 => /usr/share/man/man1/bak.1
- license.md => /usr/share/licenses/bak/LICENSE

## Dependencies

- bash
- coreutils
- tar
- zip
- unzip

## Usage

```
bak [options] <files/dirs to backup>...

	-c, --compress-using               [default: tar-gz] tar-gz, tar-xz, tar-zst, tar-bzip2, zip
		Compression format to use while creating the backup
	-C, --compute-checksums-using     [default: sha256] md5, sha1, sha224, sha384, sha256, sha512, b2
		Compute checksums for all files in the archive
	-f, --file-name                    [default: <date>.bak.<extension>]
		Name of resulting backup file
	-d, --backup-directory             [default: ~/Backups]
		Directory to place the resulting backup file in
	-e, --exclude-pattern <file/dir name/pattern to exclude>
		Pattern or name of file/dir to exclude from the archive
```

## Issues/contributing

Please feel free to open an issue on Github if the program does not work as
expected, or submit a pull request if you want to add a feature/fix a bug.

## License

This project is licensed under AGPL 3.0. A copy of the license can be found
in the [`/license.md`](./license.md) file.

```
	bak 0.2.0 - A backup tool written in bash
	Copyright (C) 2021 Vedant K (gamemaker1) \<gamemaker0042 at gmail dot com\>

	This program is free software: you can redistribute it and/or modify
	it under the terms of the GNU Affero General Public License as published by
	the Free Software Foundation, either version 3 of the License, or
	(at your option) any later version.

	This program is distributed in the hope that it will be useful,
	but WITHOUT ANY WARRANTY; without even the implied warranty of
	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
	GNU Affero General Public License for more details.

	You should have received a copy of the GNU Affero General Public License
	along with this program. If not, see https://www.gnu.org/licenses/.
```
