# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.14.2] - 2018-06-17
### Removed
- Removed the compatability check
- Disabled changing start menu objects since it uses a unique GUID

## [0.14.1] - 2018-01-01
### Added
- Missing license in class files

### Fixed
- Defender context menu not disappearing once disabled

## [0.14.0] - 2017-12-26
Ho ho ho, Merry Christmas to you all! Much work have been put to Win10Clean since it was re-written in c-sharp. This has also caused a lot of weird bugs that (IMO) I've now ironed out. Expect a GUI overhaul, reverse function and much more in 2018, again enjoy your holidays!
### Added
- Now disables the `share with` context menu, and removes the edit context menu for `.java` files
- Checks that disables the `Disable HomeGroup`, `Don't reinstall modern apps` and `Disable start menu ads` buttons if they're already applied

### Changed
- Improved the status message box when uninstalling metro apps
- Minor changes (extended error messages, code changes & improvements)
- Updated changelog information

### Fixed
- Libary folders not hidden in certian open file dialogs for amd64 users
- Missing OneDrive leftover registry key
- Broken registry paths throwing errors
- Properly lock form when doing a task

## [0.13.0] - 2017-11-18
### Added
- Re enable core Defender function if disabled
- Pin Explorer on the start menu
- Restart explorer once `Revert7` finishes
- Remove 'Pin on Start' for recycle bin
- Support for disabling print context for .url extention files
- Support for disabling modern share context menu
- Support for hiding My People in the taskbar

### Changed
- Rewritten application in C#
- Improved the update checking code, yet again
- Some changes to support v1709
- Targeting .NET 4.6.1

### Removed
- The `Disable GameDVR` button has been removed due to it being integrated in the Creators Update

## [0.12.1] - 2017-05-13
### Fixed
- Fixed the update checker

## [0.12.0] - 2017-04-17
Even more minor update this time around, brings support for the Creators Update. When I get the context menu things finished I'm going to release it as v1.
### Added
- The app list will now refresh when the `All users` checkbox state changes
- Now supporting Creators Update (removing the new Defender from startup)
- Now also disabling the `Troubleshoot compability` context menu

### Changed
- The remote server is now accessed via a secure link (GitHub have already forced HTTPS)

### Fixed
- Fixed the obvious typo (metro)
- Now removing all OneDrive tasks

## [0.11.0] - 2017-04-03
Well I'm still not dead, guess that I gotta admit that I've slowed down development a lot. The future is still bright and I will keep improving Win10Clean until the end of time :D Just that I don't have much else that I wanna implement, and am listening to feedback.
### Added
- Export console log
- Form maximum size
- Context menu cleanup improved, now also removing the following: WMP integration (image folders?!, audio files and audio folders), restoring previous version and pinning to libary

### Fixed
- Fixed OneDrive not hidden in the legacy Explorer file dialog

## [0.10.0] - 2017-02-27
### Added
- Ability to cleanup the context menu for extensions. Like printing, editing (notepad), play song and add to playlist (wmp)
- Uninstalling apps now have correct feedback (sucess, fail)
- Added removing OneDrive from Explorer file dialogs
- Added proper credit and added links to licenses

### Changed
- Improved fallback code for the update checker
- The form will now become non interactive when doing a task

### Fixed
- Prompt for uninstalling apps now tell every app to be uninstalled

## [0.9.0] - 2017-02-04
### Added
- Added a query to check if the start menu ads already has been disabled, and if so - give user choice to re-enable
- Added a fix for uninstalled apps reinstalling
- The OneDrive uninstaller now remove any leftovers found in the task scheduler
- Ability to uninstall multiple apps at once

### Changed
- Cleanup in code, now using `Using` statements in a attempt in lowering the memory usage

## [0.8.0] - 2016-11-15
### Fixed
- Fixed tab index yet again
- The OneDrive should now be sucessfully remove the icon from Explorer, and does no longer remove stuff from the registry
- Fixed a `Revert7` related error if registry key doesn't exist

## [0.7.0] - 2016-11-03
### Added
- Added support to uninstall apps installed for all users
- Replaced all forms with a big one
- Added console for extended debugging information
- Executable icon, thanks to https://github.com/Maddoc42/Android-Material-Icon-Generator

## [0.6.0] - 2016-10-02
### Added
- You can now disable HomeGroup
- Added tooltips for extended information
- Added fancy icons by famfamfam, http://famfamfam.com
- Added a about class with legal stuff
- Added option to disable home menu ads
- Pressing enter on your keyboard in the app uninstaller GUI will now act as selecting uninstall

### Changed
- A lot of actions including modifing the registry has been improved
- Improved debugging (still room for improvements, expect a debug GUI)
- When the app list for uninstalling Win10 apps is refreshed, it will save the selected app and take you back to whatever you selected - thank my friends for their feedback
- Improved Defender disabler; now removing startup process and unregistering right-click menu scans
- Improved the libary remover, the name has been changed to `Revert7` because it will now replicate the Windows 7 File Explorer settings. It now also pins the libary folder, disables quick access filling up with random crap and sets the default dir of explorer to `My PC`

### Fixed
- Fixed the tabbing index, or whenever you try to scroll the GUI using a keyboard

## [0.5.0] - 2016-09-23
Initial public release
