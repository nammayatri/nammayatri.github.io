# nammayatri.github.io

Shared notes by the Nammayatri team.

## Adding or Editing Notes

You can use VSCode or, better, [Obsidian](https://obsidian.md/) to modify this notebook. Run `nix run` locally (see below) for a live preview.

## Running using Nix

To start the live server using Nix:

```sh
nix run
```

To build the static website via Nix:

```sh
nix build -o ./result
# Then test it:
nix run nixpkgs#nodePackages.live-server -- ./result
```

## GitHub Pages

GitHub Actions CI is responsible for deploying to GitHub Pages. See `.github/workflows/publish.yaml`.
