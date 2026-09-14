# Releasing

Releases are tagged automatically by the **Tag Release** GitHub Actions workflow.

## How it works

When a commit lands on `main` that changes `elastic/.cursor-plugin/plugin.json`,
the workflow:

1. Reads the `name` and `version` from `plugin.json`.
2. Compares the version against the previous commit — if unchanged, stops.
3. Forms the tag `{name}--v{version}` (e.g. `elastic--v0.6.0`).
4. If the tag doesn't already exist, creates it and publishes a GitHub Release
   with auto-generated release notes.

## When does it run?

The workflow triggers on any push to `main` that touches
`elastic/.cursor-plugin/plugin.json`. In practice, this happens when an
agent-skills sync PR bumps the version and merges.

If the version in `plugin.json` hasn't changed (or the tag already exists),
the workflow is a no-op.

## Versioning

This plugin follows [semver](https://semver.org/):

- **Patch** (`0.0.X`): bug fixes, docs, CI changes.
- **Minor** (`0.X.0`): new skills synced, non-breaking changes.
- **Major** (`X.0.0`): breaking changes to the plugin manifest or behavior.
