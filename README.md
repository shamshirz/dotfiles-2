# RJ's Dotfiles

## Installation

1. Follow the instructions at [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) to install the thoughtbot dotfiles, but don't run `rcup` yet
2. Install these dotfiles with `git clone --recursive https://github.com/rjdellecese/dotfiles ~/dotfiles-local`
3. `rcup`
4. `brew bundle`

### Unordered

- Install a Powerline font. I use "14pt Meslo LG M Regular for Powerline", downloadable [here](https://gitbhub.com/powerline/fonts) (follow the Quick Install instructions).
- Download Tmuxinator zsh autocompletions:
```sh
curl --remote-name https://raw.githubusercontent.com/tmuxinator/tmuxinator/master/completion/tmuxinator.zsh
mv tmuxinator.zsh ~/.bin/tmuxinator.zsh
```
- Symlink `~/.config/nvim/init.vim` to `~/.vimrc`
- Install [vim-plug](https://github.com/junegunn/vim-plug) (follow installation instructions for NeoVim)

## To-Do

- Manage Ruby dependencies as well. Use Bundler? How to manage these across different Ruby versions? This is at a minimum useful/required for Tmuxinator, but is probably useful for other libraries I can't think of at time of writing.
- Prevent iTerm2 settings (and maybe other files) from being symlinked to the home directory (https://github.com/thoughtbot/dotfiles/blob/master/rcrc).
