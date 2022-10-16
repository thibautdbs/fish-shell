# AppImage builds for https://github.com/fish-shell/fish-shell

This repository contains AppImages with fish.

Features:
* it is built on `centos:7` (compatible with many old distros),
* all dependencies are statically compiled in (except glibc),
* an up-to-date terminfo database is included.

## Workflow

Releases containing AppImages are created on every push to the `add-appimage`
branch. To create a new AppImage it is sufficient to rebase this branch on a
desired commit from the upstream `master` branch and do a forced push.

*NOTE: 'Sync fork' GitHub UI feature should not be used for the `add-appimage`
branch as it creates a merge commit.*

*NOTE: Rember to sync all upstream tags, as they are used to determine the
version.*

NOTE: I asked the maintainers about providing AppImages directly in the
upstream repository but the discussion has stalled.
See: https://github.com/fish-shell/fish-shell/issues/6475#issuecomment-1165396972

