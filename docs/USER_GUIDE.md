# Snapitty User Guide

## What Snapitty Is For

Snapitty helps QA testers capture evidence while executing test cases.

Use it when you need to:

- record what happened during manual testing
- attach snaps to a batch run and test case
- export a clean evidence pack for review, audit, or handoff

It is not a test case authoring tool and it is not a defect tracker.

## Main Workflow

The normal workflow is:

1. Create a batch run
2. Add or import test cases
3. Start a case
4. Capture snaps or notes while executing
5. Retake or edit if needed
6. Mark the case outcome
7. Export the run

## The Main Areas of the App

### Workspace Window

The main workspace is where you:

- manage runs and test cases
- switch between open run tabs
- capture, paste, or note evidence
- review steps and snaps
- export finished work

### Floating Capture Window

The floating window stays available while you test in other apps.

It gives you quick access to:

- capture
- crop capture
- pause or resume
- stop current case
- finish current case
- more actions

## Creating a Batch Run

Use `New Batch Run` to start a fresh session.

Add:

- Jira or ticket reference
- run title
- build number
- environment
- test cases

If you already have cases in CSV form, import them through the run creation flow where available.

## Adding Test Cases

Test cases can be added:

- while creating a new run
- later from the test case panel

Keep case names short and readable. The export is easier to review when case titles are clean.

## Starting a Test Case

Select a case from the left panel and start it.

Once a case is active, you can:

- capture a full snap
- capture a cropped snap
- paste an image from the clipboard
- add a note-only step

## Capturing Evidence

### Full Snap

Use `Capture` to take the main configured snap type.

Depending on your current floating window switch, this may be:

- full-screen capture, or
- crop-first capture

### Cropped Snap

Use the crop button when you only want a selected region.

### Additional Snaps

If a step needs more than one image, add more snaps to the same step.

This is useful when:

- one action needs before and after evidence
- one bug needs multiple visual states
- one result needs multiple related views

### Notes

Use `Note` when you need to record context without an image.

Examples:

- response time observation
- console warning
- expected result confirmed without a visual change

## Editing Evidence

Each step or snap can be reviewed and managed inline.

Available actions may include:

- retake
- edit
- delete

When deleting from the middle of a step sequence, numbering is compacted so the list stays clean.

When deleting from the middle of a snap list, remaining snaps are renumbered.

## Retaking a Step or Snap

When you retake, Snapitty asks whether the new capture should be:

- full snap
- cropped snap

Use retake when the first capture was:

- too early
- on the wrong screen
- missing the key state
- badly framed

## Themes

Snapitty supports:

- default dark theme
- system/light theme

If your machine is on a bright desktop or you work mostly in light apps, the system theme may be easier to read.

## Timestamp Visibility

In Settings, you can control whether capture times are shown:

- inside the application
- inside exported documents

Both are currently disabled by default.

## Exporting Evidence

Snapitty currently supports Word export.

Available export modes:

- Split: one document per test case
- Combined: one document for the full run
- Hybrid: split documents plus a bundled output package

Export from the workspace using `Export...`.

## Run Library

Use `Run Library` to reopen previous work or access runs that were closed from tabs.

Closing a tab removes it from the active workspace, but the underlying run can still be reopened from the library.

## Recommended QA Usage Pattern

For the cleanest evidence packs:

1. Fill in build and environment first
2. Keep each step title short and specific
3. Use additional snaps only when they add real value
4. Use notes for things that screenshots cannot explain well
5. Retake quickly instead of leaving weak evidence in place
6. Export only after reviewing the final run

## Common Problems

### I closed a tab and it did not come back after restart

That is expected. Closed tabs are treated as intentionally closed. Reopen the run from `Run Library`.

### A thumbnail is blank or missing

Open the step or snap. If the full image exists, Snapitty should still use the main image even when a generated thumbnail is missing.

### Pytest or a local build leaves temp folders behind

That is a Windows file-locking issue during local testing, not a user-facing app issue. It does not affect normal end-user usage.

## Current Limits

- Windows-only workflow
- DOCX export only
- no built-in cloud sync
- no Jira API sync yet
- no PDF export yet

## Related Documents

- [../README.md](../README.md)
- [FUTURE_RELEASES.md](FUTURE_RELEASES.md)
- [product_roadmap.md](product_roadmap.md)
