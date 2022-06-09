<table><tr><td>
<h1 align="center"><a href="https://github.com/z-shell/zi">
  </p><img align="center" src="https://github.com/z-shell/zi/raw/main/docs/images/logo.svg" alt="Logo" width="60px" height="60px" /></a>
  ❮ ZI ❯ Package - Doctoc </p></h1>
<h2 align="center"><p> Generates table of contents for markdown files inside local git repository </p></h2>
<h3 align="center">
<table>
    <tr>
        <td><b>Package source:</b></td>
        <td>Source Tarball</td>
        <td>Binary</td>
        <td>Git</td>
        <td>Node</td>
        <td>Gem</td>
    </tr>
    <tr>
        <td><b>Status:</b></td>
        <td>❌</td>
        <td>❌</td>
        <td>❌</td>
        <td>✔️ (default)</td>
        <td>❌</td>
    </tr>
</table></h3>
<p><img align="center" src="https://user-images.githubusercontent.com/59910950/172227617-7d87bb40-d2eb-456e-ade1-1627d515d7bf.png" alt="zi doctoc package" width="100%" height="auto" /></p>
</td></tr></table><hr />

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

The [thlorenz/doctoc](https://github.com/thlorenz/doctoc) zsh package that can use the [zsh-string-lib](https://github.com/z-shell/zsh-string-lib) to automatically:

- get the plugin's Git repository OR release-package URL,
- get the list of the recommended ices for the plugin,
  - there can be multiple lists of ices,
  - the ice lists are stored in _profiles_; there's at least one profile, _default_,
  - the ices can be selectively overridden.
