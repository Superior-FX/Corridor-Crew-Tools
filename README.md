# Corridor Crew Tools

A workspace that collects Corridor Crew tools as git submodules:

| Folder | Upstream |
|---|---|
| `CK2.0_Dev` | https://github.com/nikopueringer/CK2.0_Dev |
| `CorridorKey` | https://github.com/nikopueringer/CorridorKey |
| `corridorkey-mlx` | https://github.com/nikopueringer/corridorkey-mlx |
| `Uni3CRunpod` | https://github.com/nikopueringer/Uni3CRunpod |

## Clone

```sh
git clone --recurse-submodules https://github.com/Superior-FX/Corridor-Crew-Tools.git
```

## Update every tool to its latest upstream

```sh
git submodule update --remote
git commit -am "Bump submodules"
```
