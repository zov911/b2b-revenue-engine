# Contributing

| Branch | Purpose | Merges into |
|---|---|---|
| `main` | Live site on GitHub Pages. Tagged releases only | none |
| `develop` | Next release | `main` via release PR |
| `feature/<name>` | One change | `develop` via squash PR |
| `hotfix/<name>` | Urgent fix to the live site | `main`, then back into `develop` |

1. Branch from `develop`: `git switch develop && git switch -c feature/my-change`
2. Run the checks in [docs/customize.md](docs/customize.md#check-before-you-push).
3. Open a PR into `develop`. Add a line to `CHANGELOG.md`.
4. Release: PR `develop` → `main`, then tag `vX.Y.Z`.

Any new number needs a named source in `docs/methodology.md`.
