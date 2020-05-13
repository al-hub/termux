# termux

//git
git config --global user.email "catholic2020@naver.com"
git config --global user.name "al-hub"
git config --global core.editor "vim"

//lynx config (cookies accept)
vim ~/../usr/etc/lynx.conf (linux vim /etc/lynx/lynx.cfg)
ACCEPT_ALL_COOKIES:TRUE

//tmux mouse
vim ~/../usr/etc/tmux.conf
set -g mouse on

//https://wiki.termux.com/wiki/Package_Management#Community_Repositories
curl -LO https://its-pointless.github.io/setup-pointless-repo.sh
bash setup-pointless-repo.sh


### vifm
```
tmux display-message -a  

modify imgt imagc
pane_left=$(tmux display-message -p '#{pane_left}')
pane_top=$(tmux display-message -p '#{pane_top}')

X=$(($1 + pane_left))
Y=$(($2 + pane_top))
```
