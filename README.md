<!-- markdownlint-disable MD041 -->
<div width="100%" align="center"><table>
  <tr><td align="center">
  <a title="ZI" target="_self" href="https://github.com/z-shell/zi/">
    <h2><img align="center" style="width:60px;height:auto" src="https://github.com/z-shell/zi/raw/main/docs/images/logo.svg" alt="ZI Logo" /></a>
❮ ZI ❯ Package - Doctoc </h2>
    <h3> Generates table of contents for markdown files inside local git repository. </h3>
  </td></tr><tr><td width="100%" align="center">
  <h2>

| **Package source:** | Source Tarball | Binary | Git |             Node             | Gem |
| :-----------------: | :------------: | :----: | :-: | :--------------------------: | :-: |
|     **Status:**     |      :x:       |  :x:   | :x: | :heavy_check_mark: (default) | :x: |

</h2>
<img align="center" style="width:80%;height:auto" src="https://user-images.githubusercontent.com/59910950/172227617-7d87bb40-d2eb-456e-ade1-1627d515d7bf.png" alt="Doctoc preview" />
</td></tr></table></div>

## Available `pack''` invocations

[thlorenz/doctoc](https://github.com/thlorenz/doctoc) by using the [bin-gem-node](https://github.com/z-shell/z-a-bin-gem-node) annex:

```zsh
# Download the Node package of doctoc
zi pack for doctoc
```

## Default profile

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

The [thlorenz/doctoc](https://github.com/thlorenz/doctoc) Zsh package that can use the [Zsh string library](https://github.com/z-shell/zsh-string-lib) to automatically:

-   get the plugin's Git repository OR release-package URL,
-   get the list of the recommended ices for the plugin,
    -   there can be multiple lists of ices,
    -   the ice lists are stored in _profiles_; there's at least one profile, _default_,
    -   the ices can be selectively overridden.
