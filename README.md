<h2 align="center">
  <a href="https://github.com/z-shell/zi">
    <img src="https://github.com/z-shell/zi/raw/main/docs/images/logo.svg" alt="Logo" width="80" height="80" />
  </a>
❮ ZI ❯ Package - Doctoc
</h2>

<h3 align="center">

| **Package source:** | Source Tarball | Binary | Git |             Node             | Gem |
| :-----------------: | :------------: | :----: | :-: | :--------------------------: | :-: |
|     **Status:**     |      :x:       |  :x:   | :x: | :heavy_check_mark: (default) | :x: |

</h3>

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

---

> This repository compatible with [ZI](https://github.com/z-shell/zi)

The [thlorenz/doctoc](https://github.com/thlorenz/doctoc) zsh package that can use the NPM package registry to automatically:

-   get the plugin's Git repository OR release-package URL,
-   get the list of the recommended ices for the plugin,
    -   there can be multiple lists of ices,
    -   the ice lists are stored in _profiles_; there's at least one profile, _default_,
    -   the ices can be selectively overridden.
