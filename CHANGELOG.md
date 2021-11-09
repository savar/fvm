## 2.2.4

- Ensures SDK is setup when running `use` command.

## 2.2.3

- Fix archive url from release info

## 2.2.2

- Small fix when checking for upgrade

## 2.2.1

- Fix when running flutter command with --no-version-check

## 2.2.0

- Resolves channel unknown when pulling release version
- Allows for release install of different channels [Read more](https://fvm.app/docs/advanced/release_multiple_channels)

## 2.1.1

- Removed Flutter version validation check
- Now works offline

## 2.1.0

- Removed Windows permission check

## 2.0.7

- Updated Flutter releases URL

## 2.0.6

- Added fallback if Flutter Release API is down

## 2.0.5

- Fix concurrently Flutter commands on monorepo [#296](https://github.com/leoafarias/fvm/issues/296)
- Added cli_notify to check for new version updates

## 2.0.4

- FVM only outputs information about version running when using `--verbose` [#288](https://github.com/leoafarias/fvm/issues/288)

## 2.0.3

- Fixes monorepo compatibility [#285](https://github.com/leoafarias/fvm/issues/285)

## 2.0.2

- Fixes regression when running `fvm install`

## 2.0.1

- Fix issue when retrieving settings [#281](https://github.com/leoafarias/fvm/issues/281)

## 2.0.0

- Feature: Environments - Set Flutter sdk versions per project environment.

- Feature: Doctor - Easily view the Flutter version configure for the project and configuration state

- Feature: Spawn - Easily proxy Flutter commands through any cached version

- Feature: Commits - Ability to install/use commits as the pinned SDK version.

- Feature: Custom versions - Manage custom sdk versions by add `custom_` in front of the version.

- Improvements: null-safety

- Improvements: Global - Create own command to set global versions. Deprecated "--global" flag.

- Improvements: Flutter command proxy now defaults to FVM global configured version before looking for one configured on PATH

- Improvements: Better error messaging, notifications and logging

- Improvements: Many quality of life improvements

## 1.3.8

- Issue on install [#242](https://github.com/leoafarias/fvm/issues/242)

- Auto linking[#207](https://github.com/leoafarias/fvm/issues/207)

## 1.3.7

- Fix issue for delay exist after use command [#195](https://github.com/leoafarias/fvm/issues/195)

## 1.3.6

- Enhancement: Added PATH env on Flutter processs. For better third party tooling support.

- Fix: Updated Grinder dependencies

- Fix: Better ancestor lookup logic for monorepo setups. [#180](https://github.com/leoafarias/fvm/issues/180)

## 1.3.5+1

- Added symlink on install behavior without version
- Clean up

## 1.3.4

- Better support for CI, and custom workflows using `fvm flutter ...` commands.

## 1.3.3

- Fix error when setup on some platforms and tools [#160](https://github.com/leoafarias/fvm/issues/160)

## 1.3.2

- Better logging for Flutter setup.

## 1.3.1

- Fix issue when running `install` command with pinned version [#161](https://github.com/leoafarias/fvm/issues/161)

## 1.3.0

- Bug fixes and improvements 😂

- Implemented ability to change cachePath` on settings [#101](https://github.com/leoafarias/fvm/issues/101)

- Improved UX with Flutter run command [#124](https://github.com/leoafarias/fvm/issues/124)

- Added a notice on Windows to run as developer mode or administrator

- Ability to set Flutter Git Repo URL (Advanced)

## 1.2.3

- Clone setting changes. Unexpected behavior when installing master in some cases

## 1.2.2

- Updated process_run dependency (Issue #113)

## 1.2.0

- Use command now shows the installed version if no 'version' is passed.
- Improved exception message handling

## 1.1.9

- Improvements on flutter channels parsing

## 1.1.8

- Fix for shared releases between channels

## 1.1.7

- Changed version on builder

## 1.1.6

- Better support for Windows

## 1.1.5

- Added message with notice and fix if Flutter releases URL is blocked in your country.

## 1.1.4

- Nested FVM config look up, to be used on monorepo projects, or nested directories.
- Added link to changelog on upgrade message.

## 1.1.3

- Removed Flutter project guard from flutter proxy command

## 1.1.2

- Added upgrade message if not running the latest fvm version

## 1.1.1

- Static analysis, and dart convention on README.md

## 1.1.0

- Implemented --force flag on `use` command to bypass guards if needed.
- Set where fvm caches versions using FVM_HOME environment variable
- Deprecated --cache-path in favor of FVM_HOME

## 1.0.4

- Indicates global version on list command.

## 1.0.3

- Fixes issue with stdin on Flutter commands.

## 1.0.2

- Indicates channels on `fvm releases` command.

## 1.0.1

- Suppress verbose message for install progress.

## 1.0.0

- List Flutter Releases
- Bug fixes and optimization
- Project refactoring

## 0.8.3

- Installation progress output
- Flutter setup on installation
- Ability to skip setup with`--skip-setup`

## 0.8.2

- Size optimization of SDK downloads
- Code clean-up

## 0.8.1

- Fixes `list` command when project has no config.

## 0.8.0

- Implemented `--global` flag to set a specific version globally.
- Changed project configuration to allow for versioning.
- Refactoring and project clean-up
- Better user experience
- Improved error messages

## 0.7.2

- Better compatibility with flutter commands.

## 0.7.1

- Updated version constant

## 0.7.0

- Added support for new Flutter 1.17.0+ [versioning scheme](https://groups.google.com/forum/#!msg/flutter-announce/b_EcYtyo8Q4/2QSfdp2aBwAJ) -
  The new versioning scheme includes changes to tag names and thus also version names for FVM. When reinstalling Flutter versions <1.17.0, the FVM install-path will change, potentially breaking projects that rely on the install-path.
  The install-path will change from `~/fvm/versions/1.15.17` to `~/fvm/versions/v1.15.17`. Make sure to change this in your IDE configuration.

## 0.6.7

- Added `version` command to see currently installed `fvm` version

## 0.6.6

- Better Flutter command compatibility
- Improved error logging and --verbose behavior
- Friendlier error messages

## 0.6.5

- Better Error handling and friendlier error message

## 0.6.4

- Project clean-up and tweaks for better pub analysis.

## 0.6.3

- Initial stable version rewritten in Dart.
