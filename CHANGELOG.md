# Changelog

All notable changes to Snapitty should be recorded in this file.

## [0.2.1] - 2026-04-25

### Changed

- Bumped release version to `0.2.1`.
- Corrected installer and shortcut references to `Snapitty.exe`.
- Updated public release documentation.
- Improved New Batch Run wizard theme consistency.

### Fixed

- Fixed inconsistent app and uninstall icon handling.
- Fixed low-contrast New Batch Run wizard header text.
- Removed deprecated UTC timestamp warnings.

### Notes

- Windows may cache old app icons after reinstall. Restart Explorer or refresh the icon cache if needed.
- Snapitty remains freeware for personal, internal, and commercial QA use, but is not open source.


## [0.2.0] - 2026-04-25

### Added

- Floating capture widget with full snap and cropped snap switching
- Multi-tab batch run workspace
- Run Library and archived run reopening flow
- Clipboard paste into evidence
- Note-only steps
- Multi-snap support within a single step
- Step and snap retake, edit, and delete actions
- Export modes for split, combined, and hybrid DOCX output
- System/light theme support in addition to the default dark theme
- Settings for showing capture times in app and export

### Changed

- Reworked icon usage across the main window, floating widget, and dialogs
- Improved contrast and border visibility in dark and light themes
- Reworked evidence list row layout to reduce overlap and clutter
- Closed tabs no longer auto-reopen on next launch unless explicitly reopened from Run Library
- Visible terminology is moving toward "snap" instead of "screenshot" where appropriate

### Fixed

- Evidence row overlap and duplicated thumbnail text
- Thumbnail fallback handling when generated thumbnails are missing
- Tab close button visibility
- UTC timestamp generation updated to timezone-aware UTC to remove deprecation warnings

## [0.1.0] - 2026-04-22

### Added

- Initial working Snapitty desktop build
- Local workspace, test case execution flow, and DOCX export baseline
