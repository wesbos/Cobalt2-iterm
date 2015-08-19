# Cobalt2 for iTerm2 and ZSH

Two things for lovers of the [Sublime Text Theme](https://github.com/wesbos/cobalt2). Cobalt2 in your terminal!

![](http://wes.io/Ub3k/content)

`cobalt2.itermcolors` is for anyone who uses iTerm2 and wants the colours. The `cobalt2.zsh-theme` is the prompt layout for zsh users. 

They work well together! You will need to install the patched powerline font as well: <https://github.com/powerline/fonts>

####Step-by-step installation
1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
2. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.
3. In iTerm2 access the *Preferences* pane on the *Profiles* tab.
4. Under the *Colors* tab import the `cobalt2.itermcolors` file via the *Load Presets* drop-down.
5. Under the *Text* tab change the font for each type (*Regular* and *Non-ASCII*) to '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
6. Refresh ZSH by typing `source ~/.zshrc` on the command line.

##### ...in a MinTTY environment
1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
2. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.
3. Install '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
4. Replace the `~/.minttyrc` file with the `.minttyrc` file in this repo.
5. Restart your terminal. 