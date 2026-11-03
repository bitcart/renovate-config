# Bitcart Renovate config

This repository contains configuration defaults shared between all our repositories using Renovate.

[Renovate](https://renovatebot.com) is used for dependency updates to ensure that our software and related packages always use the latest features and have no security vulnerabilities.

## Presets

Extend one of them from the repository's `.github/renovate.json`:

| Preset                                | For                                                                  | Behaviour                                                                                                          |
| ------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| `local>bitcart/renovate-config`       | Actively developed repositories                                      | Weekly grouped non-major PR; majors and Python lock file maintenance wait for approval on the Dependency Dashboard |
| `local>bitcart/renovate-config:audit` | Repositories where a merge reaches production, or that rarely change | Every update waits for approval on the Dependency Dashboard; security updates still open PRs on their own          |

## Copyright and License

Copyright (C) 2021 MrNaif2018

Licensed under the [MIT license](LICENSE)
