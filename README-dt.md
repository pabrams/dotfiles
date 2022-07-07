# .dotfiles Readme

## setup
git init --bare $HOME/.cfg
alias dt='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
dt config --local status.showUntrackedFiles no
echo "alias dt='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc

## add
dt status
dt add /home/me/.dotfiles/README.md
