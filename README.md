# Snapitty

Snapitty is a Windows desktop application for QA evidence capture.

It is built for testers who need to:

- capture full-screen or cropped snaps quickly
- organise evidence by batch run and test case
- add notes while executing
- review and retake snaps without rebuilding a case
- export the result as Word evidence packs

Snapitty is intentionally focused. It is not a full test management product. It works alongside Jira, TestRail, Zephyr, spreadsheets, or any existing QA workflow.

## Current Release

- App version: `0.2.0`
- Installer script version source: [installer/Snapitty.iss](installer/Snapitty.iss)
- Packaged installer output pattern: `Snapitty-Setup-0.2.0.exe`

Release history is tracked in [CHANGELOG.md](CHANGELOG.md).

## Tech Stack

- Python 3.14
- PySide6 for the desktop UI
- SQLite for local storage
- Pillow and MSS for capture and image handling
- python-docx for export generation
- PyInstaller for packaging
- Inno Setup for the Windows installer

## Main Capabilities

- Batch run workspace with multiple tabs
- Floating capture window
- Full snap and cropped snap capture modes
- Clipboard image paste into evidence
- Note-only steps
- Step retake, edit, reorder, and delete
- Multi-snap support under one step
- Run Library and archived workspace access
- DOCX export in split, combined, and hybrid modes
- Dark theme plus system/light theme support

## Requirements

Development and packaging are currently aimed at Windows.

Recommended environment:

- Windows 11

## App Documentation

User-facing documentation lives here:

- [docs/USER_GUIDE.md](docs/USER_GUIDE.md)
- [docs/FUTURE_RELEASES.md](docs/FUTURE_RELEASES.md)

## License

Snapitty is not open source.

It is currently positioned as a privately distributed freeware/commercial-use application with protected branding, packaging, and redistribution boundaries.

See [LICENSE.txt](LICENSE.txt) for the full license.

Short version:

- users may use the official app for QA work
- user-created screenshots and exports belong to the user or organisation
- source modification, rebranding, altered redistribution, and resale are not permitted without written permission

## Planned Direction

The higher-level product direction is documented in [docs/FUTURE_RELEASES.md](docs/FUTURE_RELEASES.md) and [docs/product_roadmap.md](docs/product_roadmap.md).
