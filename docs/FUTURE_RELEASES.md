# Future Releases

This document is intended for the GitHub repository and product planning. It is not a strict commitment. It is a practical direction for future Snapitty releases.

## Product Position

Snapitty should stay focused on evidence capture for manual QA.

It should continue to be:

- fast to open
- easy to capture with
- simple to review
- professional to export

It should avoid turning into a full test management suite.

## Release Direction

## Version 0.3.x

Focus: polish, visibility, and everyday QA convenience.

Possible additions:

- stronger export review flow before final generation
- improved inline title editing
- better handling for failed and blocked case notes
- richer run metadata in the workspace and export
- more robust archive browsing and reopen flow
- additional thumbnail recovery and media validation

## Version 0.4.x

Focus: export quality and evidence completeness.

Possible additions:

- export cover page with build, environment, tester, and summary
- expected versus actual result fields
- defect reference fields for failed cases
- better run-level notes
- cleaner handling of setup or precondition evidence
- optional PDF export

## Version 0.5.x

Focus: advanced QA workflows.

Possible additions:

- countdown or delayed capture
- per-capture monitor switching
- blur or redact annotation tools
- export preview
- richer archive packaging
- custom export templates

## Version 1.0.0

Focus: a stable, well-documented private release suitable for broader team rollout.

Suggested goals:

- consistent UI wording and documentation
- stable installer and upgrade path
- strong export reliability
- clear licensing and distribution rules
- tested reopen and archive flow
- polished user guide

## Features Worth Considering

### High-value additions

- defect ID and summary support
- export summary page
- run-level notes
- redact or blur tool
- PDF export
- Jira attachment handoff

### Nice-to-have additions

- more export naming presets
- better capture routing for quick one-off work
- keyboard shortcut customisation
- richer archive search
- better diagnostics for missing images or corrupted runs

## Things Snapitty Should Probably Not Become

To keep the product useful and maintainable, avoid turning it into:

- a test case management platform
- a defect tracker
- a team permission system
- a CI reporting dashboard
- a browser automation framework

## Release Checklist Template

For each new version:

1. update `MyAppVersion` in `installer\Snapitty.iss`
2. update `CHANGELOG.md`
3. run tests
4. build PyInstaller output
5. build installer
6. smoke-test install and launch
7. verify export
8. tag release in Git
9. push to private GitHub repository

## Distribution Notes

Because this is not an open-source project:

- keep the GitHub repository private
- keep internal planning docs that should remain private out of public release packages if needed
- review screenshots or sample data before every push
- keep installer and license wording aligned
