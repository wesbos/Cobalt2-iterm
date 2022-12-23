# Cobalt2 for iTerm2 and ZSH

<img width="664" alt="iTerm2 Cobalt2" src="https://user-images.githubusercontent.com/176013/209395069-7e307ba0-d645-40d7-a235-267a9430080e.png">

* `cobalt2.itermcolors` is Cobalt2 theme for iTerm2 - This makes things blue and yellow.
* `cobalt2.zsh-theme` is the custom prompt for oh-my-zsh. It makes that cool line with folder and git status. 

They work well together! You will need to install the patched powerline font as well: <https://github.com/powerline/fonts>

#### Step-by-step installation
1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
2. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.

3. Install Powerline and necessary fonts, one way is using [PIP](https://en.wikipedia.org/wiki/Pip_(package_manager))
 * For first time *PIP* users refer to this [PIP installation guide](https://pip.pypa.io/en/stable/installing/)
 * To install Powerline using pip
  ```
pip install --user powerline-status
  ```
 * Now install all necessary fonts by downloading or cloning git repository.

  ```
git clone https://github.com/powerline/fonts
cd fonts
./install.sh
  ```
  
> note: if you are using iTerm2, they now have a checkbox for Powerline fonts `Profiles` → `Text`.

3. In iTerm2 access the *Preferences* pane on the *Profiles* tab.
4. Under the *Colors* tab import the `cobalt2.itermcolors` file via the *Load Presets* drop-down.
5. Under the *Text* tab change the font for each type (*Regular* and *Non-ASCII*) to '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
6. Refresh ZSH by typing `source ~/.zshrc` on the command line.
7. If you want the full blown tabs and everything shown in the screenshot, use the Profile in Cobalt2.json.

##### ...in a MinTTY environment
1. Drop the `cobalt2.zsh-theme` file in to the `~/.oh-my-zsh/themes/` directory.
2. Open up your ZSH preferences at `~/.zshrc` and change the theme variable to `ZSH_THEME="cobalt2"`.
3. Install '**Inconsolata for Powerline**'. (Refer to the [powerline-fonts repo](https://github.com/powerline/fonts) for help on font installation.)
4. Replace the `~/.minttyrc` file with the `.minttyrc` file in this repo.
5. Restart your terminal.

#### Visual Studio Code Settings
By default VSCode integrated terminal won't be able to pick the powerline fonts directly.To make this work, you need to update the integrated terminal font family property.Follow the steps below:
1. Open VS Code preference settings(`[CMD + ,]` for macOS).
2. Add the following key to the user settings
  `"terminal.integrated.fontFamily": "Inconsolata for Powerline"`
3. Save and Restart.