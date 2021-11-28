<h3>

| **Package source:** | Source Tarball | Binary | Git |             Node             | Gem |
| :-----------------: | :------------: | :----: | :-: | :--------------------------: | :-: |
|     **Status:**     |      :x:       |  :x:   | :x: | :heavy_check_mark: (default) | :x: |

</h3>

- [Introduction](#introduction)
- [Install](#install)
	- [Available `pack''` invocations](#available-pack-invocations)
	- [Default Profile](#default-profile)

# Introduction

> **[?]**
> This repository not compatible with previous versions (zplugin, zinit).
>
> Please upgrade to [ZI](https://github.com/z-shell-zi)

The [thlorenz/doctoc](https://github.com/thlorenz/doctoc) zsh package than can use the NPM package registry to automatically:

-   get the plugin's Git repository OR release-package URL,
-   get the list of the recommended ices for the plugin,
    -   there can be multiple lists of ices,
    -   the ice lists are stored in _profiles_; there's at least one profile, _default_,
    -   the ices can be selectively overridden.

# Install

## Available `pack''` invocations

[thlorenz/doctoc](https://github.com/thlorenz/doctoc) by using the [bin-gem-node](https://github.com/z-shell/z-a-bin-gem-node) annex:

```zsh
# Download the Node package of doctoc
zi pack for doctoc
```

## Default Profile

Provides the CLI command `doctoc`.

The Node packages are installed locally into a null-plugin directory (feature of the bin-gem-node annex) and provided to the command line through _shims_,
i.e.: automatic forwarder scripts created under `$ZPFX/bin` (which is added to the `$PATH` by default; shims are also a bin-gem-node annex feature).

The ZI command executed will be equivalent to:

```zsh
zi lucid as=null node="!doctoc" sbin="n:node_modules/.bin/doctoc" for \
    z-shell/null
```
