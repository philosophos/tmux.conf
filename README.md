#### Install    
###### install tmux    
deb-based distro(Debian,Ubuntu,Mint,etc):    
&emsp;`apt-get install tmux`    
&emsp;or    
&emsp;`aptitude install tmux`    
rpm-based distro(Redhat,CentOS,Fedora,etc):    
&emsp;`yum install tmux`    
&emsp;or    
&emsp;`dnf install tmux`    
Arch Linux:    
&emsp;`pacman -S tmux`    
&emsp;or    
&emsp;`yaourt -S tmux`    
    
###### install rainbarf    

    cd /tmp    
    git clone https://github.com/creaktive/rainbarf.git    
    cd rainbarf-master/    
    perl build.pl    
    ./build test    
    ./build install    
###### install tmux-mem-cpu-load    

    cd /tmp    
    git clone https://github.com/thewtex/tmux-mem-cpu-load.git    
    cd tmux-mem-cpu-load/    
    cmake .    
    make    
    su -c 'make install'    
###### install the configuration    

    git clone https://github.com/philosophos/tmux.conf    
copy .tmux.conf to your home dir    
    
    
#### ShortKey Change:    
    
C-x   &emsp;send-prefix  
C-F5  &emsp;source-file ~/.tmux.conf \; display "TMUX Config Reloaded!"

x     &emsp;lock-server  
Q     &emsp;kill-session

\-    &emsp;Split the current pane into two, top and bottom.  
\     &emsp;Split the current pane into two, left and right.
    
###### Resize the current pane in steps of one cell.    
C-k &emsp;upward    
C-j &emsp;downward    
C-h &emsp;to the left    
C-l &emsp;to the right    
    
###### Move between panel    
k &emsp;up    
j &emsp;down    
h &emsp;left    
l &emsp;right    
, &emsp;previous-window  (<)    
. &emsp;next-window      (>)    
    
###### cope mode    
p &emsp;paste buffer (prefix Ctrl+p):Paste the most recently copied buffer of text.    
v &emsp;begin-selection:Enter copy mode to copy text or view the history.    
y &emsp;copy-selection    
  
  
#### One More Thing  
if you wang to change the tmux's color configuration,there is [a bash script](
https://github.com/philosophos/show256color)  I wrote,which can show 256color   
in terminal.  
