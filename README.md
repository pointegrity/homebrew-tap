# pointegrity/homebrew-tap

Homebrew tap for [Pointegrity](https://pointegrity.com) tools.

## poi

**poi keeps an id-anchored record beside your code** — the part of a project that
was *decided* rather than written: why it is this way and not that way, what must
stay true, and what has already bitten someone here.

```sh
brew install pointegrity/tap/poi
```

Source and documentation: [pointegrity/poi](https://github.com/pointegrity/poi)

## About the casks here

Everything in `Casks/` is **generated on release by GoReleaser** — edit the
source repository, not this one. Hand edits are overwritten by the next release.

poi ships as a cask rather than a formula because it is a pre-compiled binary.
The cask's `postflight` clears the macOS quarantine attribute, which is what
otherwise reports *"poi cannot be opened because the developer cannot be
verified"* on first run. That is a workaround for the binaries not yet being
notarised, not a substitute for it.

## Licence

The tools distributed through this tap carry their own licences; see each
project. **METHOD**, the spec discipline poi enforces, is CC BY 4.0 and ships
inside every poi archive.
