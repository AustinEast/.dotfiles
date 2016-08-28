# dotfiles
My install files.

Takes advantage of [Mackup](https://github.com/lra/mackup) to store config files on Dropbox.

# Instructions

1. `zsh`
2. `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. `brew install rcmdnk/file/brew-file`
4. `brew file set_repo`
5. `brew file install`
6. `git clone --recursive https://github.com/AustinEast/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"`
7. `setopt EXTENDED_GLOB`
8. `for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do`
9. `ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"`
10. `done`
11. `chsh -s /bin/zsh`
12. Restart Terminal
13. Sign into Dropbox and start syncing. Take a walk outside or eat a snack while waiting.
14. Once Dropbox is done syncing: `mackup restore`
