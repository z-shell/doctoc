# `THLORENZ/DOCTOC` ZINIT PACKAGE

## Homepage link: [thlorenz/doctoc](https://github.com/thlorenz/doctoc)

| **Package source:** | Source Tarball | Binary | Git |       Node       | Gem |
|:-------------------:|:--------------:|:------:|:---:|:----------------:|:---:|
|     **Status:**     |       -        |   -    |  -  | + <br> (default) |  –  |

[Zinit](https://github.com/z-shell/zinit) can use the NPM package registry
to automatically:

- get the plugin's Git repository OR release-package URL,
- get the list of the recommended ices for the plugin,
  - there can be multiple lists of ices,
  - the ice lists are stored in *profiles*; there's at least one profile, *default*,
  - the ices can be selectively overriden.

Example invocations that'll install
[thlorenz/doctoc](https://github.com/thlorenz/doctoc) by using the
[bin-gem-node](https://github.com/z-shell/z-a-bin-gem-node) annex:

```zsh
# Download the Node package of doctoc
zinit pack for doctoc
```

## Default Profile

Provides the CLI command `doctoc`.

The Node packages are installed locally into a null-plugin directory (feature of
the bin-gem-node annex) and provided to the command line through *shims*, i.e.:
automatic forwarder scripts created under `$ZPFX/bin` (which is added to the
`$PATH` by default; shims are also a bin-gem-node annex feature).

The Zinit command executed will be equivalent to:

```zsh
zinit lucid as=null node="!doctoc" sbin="n:node_modules/.bin/doctoc" for \
    z-shell/null
```

<!-- vim:set ft=markdown tw=80 fo+=an1 autoindent: -->
