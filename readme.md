# Cobalt2 for iTerm2 and ZSH

Two things for lovers of the [Sublime Text Theme](https://github.com/wesbos/cobalt2). Cobalt2 in your terminal!

![](http://wes.io/Ub3k/content)

`cobalt2.itermcolors` is for anyone who uses iTerm2 and wants the colours. The `cobalt2.zsh-theme` is the prompt layout for zsh users. 

They work well together! You will need to install the patched powerline font as well: <https://github.com/powerline/fonts>

## Step-by-step installation

1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
1. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.
1. Install Powerline and necessary fonts, one way is using [PIP](https://en.wikipedia.org/wiki/Pip_(package_manager)):
    - For first time *PIP* users refer to this [PIP installation guide](https://pip.pypa.io/en/stable/installing/)
    - To install Powerline using pip
    ```
    pip install --user powerline-status
    ```
    - Now install all necessary fonts by downloading or cloning git repository.
    ```
    git clone https://github.com/powerline/fonts
    cd powerline
    ./install.sh
    ```
1. In iTerm2 access the *Preferences* pane on the *Profiles* tab.
1. Under the *Colors* tab import the `cobalt2.itermcolors` file via the *Load Presets* drop-down.
1. Under the *Text* tab change the font for each type (*Regular* and *Non-ASCII*) to '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
1. Refresh ZSH by typing `source ~/.zshrc` on the command line.

### ...in a MinTTY environment

1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
1. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.
1. Install '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
1. Replace the `~/.minttyrc` file with the `.minttyrc` file in this repo.
1. Restart your terminal.
