# Fork Ranger content

This repository publishes the content used by current versions of Fork Ranger.

## Source of truth

Content changes must be made in the legacy
[`jordibruin/forkrangerRecipes`](https://github.com/jordibruin/forkrangerRecipes)
repository. A GitHub Actions workflow mirrors its `main` branch into this
repository's `main` branch every hour, on the hour (UTC). The workflow can also
be started manually from the Actions tab.

Do not edit mirrored content directly in this repository. Such edits are removed
the next time the mirror workflow runs.

## Files maintained here

The mirror deliberately preserves these new-repository-only files:

- `.github/`, including the mirror workflow itself
- `.last-sync-sha`, which records the mirrored legacy commit
- `README.md`, this documentation

Every other tracked path is replaced with the exact contents of the legacy
repository. This includes upstream file additions, modifications, and deletions.
