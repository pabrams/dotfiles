# .dotfiles Readme

## setup
git init --bare $HOME/.cfg
alias dt='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
dt config --local status.showUntrackedFiles no
echo "alias dt='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc

## add README
dt status
dt add /home/me/README-dt.md
dt commit -m "add README"
dt push

## add .zshrc
dt add .zshrc
dt commit -m "add zshrc"
dt push
