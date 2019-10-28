# [omz][repo-link]
> A simplistic plugin manager for [oh-my-zsh][omz-link] using pure zsh scripts.
> Inspired by oh-my-fish's default plugin manager.

[![MIT License](https://img.shields.io/github/license/redxtech/omz)](/LICENSE)
[![oh-my-zsh](https://img.shields.io/github/stars/robbyrussell/oh-my-zsh?label=oh-my-zsh)][omz-link]

## install

```zsh
git clone https://github.com/redxtech/omz.git $ZSH_CUSTOM/plugins/omz
```

## features

* clone plugins from github
* update plugins
* update all plugins at once
* remove plugins
* load plugins (without oh-my-zsh)

## usage

### add a plugin
```zsh
# github username & repo of the plugin
omz add username/repo
```

You will still have to load the plugin manually. See below.

### update a plugin
```zsh
# omit the plugin repo path to update all plugins
omz update username/repo
```

### remove a plugin
```zsh
# github username & repo of the plugin
omz remove username/repo
```

You will still have to remove the plugin from the plugin list manually.

### load a plugin
```zsh
# within your .zshrc (before sourcing oh-my-zsh.sh)
# with the plugin name being the github repo without username
plugins=(
    ...
    plugin-name
)
# OR
# anywhere in the shell
# github username & repo of the plugin
omz load username/repo
```

## author

**omz** © [redxtech][author], released under the [MIT][mit] license.

[mit]:              https://opensource.org/licenses/MIT
[author]:           https://github.com/redxtech
[omz-link]:         https://github.com/robbyrussell/oh-my-zsh
[repo-link]:        https://github.com/redxtech/omz

