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


//[403 issue](https://knowledgeinfinteloop.blogspot.com/2021/09/100-fixed-termux-all-errors-403.html)  
**termux-change-repo**   
→ select "science repository" and press "ok"  
→ select "Mirror by Grimle" option and again press "ok"   
→ apt upgrade  → apt update  

### vifm  
```
tmux display-message -a  

modify imgt imagc  
vim .config/vifm/scripts/imgt  
vim .config/vifm/scripts/imgc  
  
pane_left=$(tmux display-message -p '#{pane_left}')  
pane_top=$(tmux display-message -p '#{pane_top}')  
  
X=$(($1 + pane_left))  
Y=$(($2 + pane_top))  
```


### vnc  
prepare  
-.Andronix  
-.VNC Viewer  

BASIC connect
```
1. install linux(as ubuntu) by Andronix (takes about 20~30 minutes)
2. run linux script ( as ./start-ubuntu20.sh )
3. check VNC SERVER 
   vncserver -list  
   nvcserver-stop  
   vncserver-start  
4. open VNC Viewer
5. access it as localhost:5901
   
```
