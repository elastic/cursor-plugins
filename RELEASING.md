# Releasing

Releases are tagged automatically by the **Tag Release** GitHub Actions workflow.

## How it works

When a commit lands on `main` that changes `elastic/.cursor-plugin/plugin.json`,
the workflow:

1. Reads the `version` from `plugin.json`.
2. Uses the version as the tag (e.g. `0.6.0`).
3. Creates the git tag if it doesn't already exist.
4. Creates a GitHub Release if one doesn't already exist for that tag.

## When does it run?

The workflow triggers on any push to `main` that touches
`elastic/.cursor-plugin/plugin.json`. In practice, this happens when an
agent-skills sync PR bumps the version and merges.

If the tag and release already exist for the current version, the workflow
is a no-op. This makes re-runs safe — if the tag was created but the release
step failed, re-running will skip tag creation and pick up at release creation.

## Versioning

This plugin follows [semver](https://semver.org/):

- **Patch** (`0.0.X`): bug fixes, docs, CI changes.
- **Minor** (`0.X.0`): new skills synced, non-breaking changes.
- **Major** (`X.0.0`): breaking changes to the plugin manifest or behavior.
