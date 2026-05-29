# Modifications by SeeYouLink, Inc.

This fork of the upstream `syncit` project (https://github.com/Yuyz0112/syncit, also mirrored at https://github.com/rrweb-io/syncit) contains modifications by SeeYouLink, Inc. and is provided as part of the Talaria platform.

**Upstream project:** syncit
**Upstream URL:** https://github.com/Yuyz0112/syncit
**Upstream license:** MIT (as declared in upstream `package.json`; the upstream repository does not ship a separate LICENSE file)
**Fork maintainer:** SeeYouLink, Inc.
**Fork URL:** https://github.com/talaria-dev/syncit
**Modification period:** January 2022 to present

## Summary of modifications

SeeYouLink's modifications to the `syncit` fork are minimal and operational in nature. No changes have been made to the core source code of any `syncit` package, and the public API surface of the upstream library is fully preserved.

The modifications consist of:

- **Routine dependency installation** — `yarn install` was run to materialize the `node_modules` tree and update `yarn.lock` for the SeeYouLink build environment.
- **Restated `LICENSE` file** — The upstream `syncit` repository declares the MIT License in its `package.json` but does not ship a standalone `LICENSE` file. SeeYouLink added a `LICENSE` file restating the MIT license declared by the upstream maintainers, with a second copyright line covering the SeeYouLink fork. The full text of `LICENSE` documents the rationale.

The `syncit` source code itself has not been modified by SeeYouLink. The `talaria-client` package consumes the `syncit` UI library as a runtime dependency and bundles its compiled output (see `talaria-client/libs/syncit/`); the source repository here remains a clean fork of upstream.

## Modified files

- `LICENSE` (added; restates upstream-declared MIT license; see file header for rationale)
- `yarn.lock` (regenerated as part of `yarn install`)

The following files appear in the modification history as `.DS_Store` artifacts created by macOS Finder during local development; they are not substantive code changes and may be removed in any future cleanup:

- `.DS_Store`, `packages/.DS_Store`, `packages/core/.DS_Store`, `packages/transporter/.DS_Store`

## Commit history

The complete history of SeeYouLink modifications is preserved in the fork's git log:

```
git log --author="Zoran" --author="Talaria" --oneline
```

All upstream commit history is preserved and unmodified.

## Compliance statement

This `MODIFICATIONS.md` is provided as a clear, prominent notice that SeeYouLink, Inc. has modified files in this fork. The upstream-declared MIT license is preserved and restated in `LICENSE`. Redistribution of this fork in source or binary form must continue to comply with the MIT license terms; the upstream copyright notice (Yanzhen Yu and syncit contributors) and the SeeYouLink fork copyright are both preserved.
