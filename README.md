# Tmux config
This is my tmux configuration and I've created this repository to keep a portable configuration for my tmux.
In the `tmux.conf` all references, inspirations and credits are avilable, e.g. sessionizer is an idea of The Primeagen that I really liked and wanted to bring in my workflow.

# Requirements
To make this configuration working some dependencies are required:
- [fzf](https://github.com/junegunn/fzf)

# Installing
Type in your terminal 
```bash
$ git clone https://github.com/cedrata/tmux.conf.git ~/.config/tmux
```

Once the directory is cloned append the following content to your `.zshrc` or `.bashrc` replacing the values of `TSESH_DIRS` with the directories where you want to apply the `find` command.
```bash
# tmux variables
export TSESH_DIRS="$HOME/Dev $HOME/.config"
tmux set-environment -g TSESH_DIRS "$TSESH_DIRS"

```
Those are required in order to make the script sessionizer script work properly.

Now you're ready to go!
