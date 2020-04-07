# Ansible role - xdg

Role for configuring stubborn programs to follow
[xdg base directory specification](https://wiki.archlinux.org/index.php/XDG_Base_Directory)
using environment variables.

## Details
1. XDG base directories are created if do not exist
2. Below variables are set in configs of specified shells (`fish`, `bash`, `zsh`):

variable | value
--- | ---
`BASH_COMPLETION_USER_FILE` | `$XDG_CONFIG_HOME/bash-completion/bash_completion`
`LESSHISTFILE` | `$XDG_DATA_HOME/lesshst`
`CARGO_HOME` | `$XDG_DATA_HOME/cargo`
`RUSTUP_HOME` | `$XDG_DATA_HOME/rustup`
`JUPYTER_CONFIG_DIR` | `$XDG_CONFIG_HOME/jupyter`
`IPYTHONDIR` | `$XDG_CONFIG_HOME/ipython`
`PYTHON_EGG_CACHE` | `$XDG_CACHE_HOME/python-eggs`
`NODE_REPL_HISTORY` | `$XDG_DATA_HOME/node_repl_history`
`NPM_CONFIG_USERCONFIG` | `$XDG_CONFIG_HOME/npm/npmrc`
`MYSQL_HISTFILE` | `$XDG_DATA_HOME/mysql_history`
`_JAVA_OPTIONS` | `-Djava.util.prefs.userRoot=$XDG_CONFIG_HOME/java`
`DOCKER_CONFIG` | `$XDG_CONFIG_HOME/docker`
`MACHINE_STORAGE_PATH` | `$XDG_DATA_HOME/docker-machine`
`GTK_RC_FILES` | `$XDG_CONFIG_HOME/gtk-1.0/gtkrc`
`GTK2_RC_FILES` | `$XDG_CONFIG_HOME/gtk-2.0/gtkrc`
`TERMINFO` | `$XDG_DATA_HOME/terminfo`
`TERMINFO_DIRS` | `$XDG_DATA_HOME/terminfo:/usr/share/terminfo`
`XCOMPOSEFILE` | `$XDG_CONFIG_HOME/X11/xcompose`
`XCOMPOSECACHE` | `$XDG_CACHE_HOME/X11/xcompose`
`GNUPGHOME` | `$XDG_DATA_HOME/gnupg`
`TMUX_TMPDIR` | `$XDG_RUNTIME_DIR`
`WINEPREFIX` | `$XDG_DATA_HOME/wineprefixes/default`  # MUST BE CREATED
`VAGRANT_HOME` | `$XDG_DATA_HOME/vagrant`
`VAGRANT_ALIAS_FILE` | `$XDG_DATA_HOME/vagrant/aliases`
