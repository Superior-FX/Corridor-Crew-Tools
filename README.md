# Corridor Crew Tools

A workspace that collects Corridor Crew tools as git submodules. Each submodule
points at a Superior-FX fork, so changes can be pushed; the original repos are
kept as an `upstream` remote.

| Folder | Fork | Original |
|---|---|---|
| `CK2.0_Dev` | https://github.com/Superior-FX/CK2.0_Dev | https://github.com/nikopueringer/CK2.0_Dev |
| `CorridorKey` | https://github.com/Superior-FX/CorridorKey | https://github.com/nikopueringer/CorridorKey |
| `corridorkey-mlx` | https://github.com/Superior-FX/corridorkey-mlx | https://github.com/nikopueringer/corridorkey-mlx |
| `Uni3CRunpod` | https://github.com/Superior-FX/Uni3CRunpod | https://github.com/nikopueringer/Uni3CRunpod |

## Clone

```sh
git clone --recurse-submodules https://github.com/Superior-FX/Corridor-Crew-Tools.git
```

## Pull in changes from an original repo

```sh
cd CorridorKey
git remote add upstream https://github.com/nikopueringer/CorridorKey.git  # once, on a fresh clone
git fetch upstream && git merge upstream/main && git push
cd .. && git commit -am "Bump CorridorKey" && git push
```

`gh repo sync Superior-FX/<repo>` does the same merge on GitHub without a local checkout.
