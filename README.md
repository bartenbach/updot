#updot
--------------
![Screenshot.png](http://i.imgur.com/TceUS.png)
--------------
###description
updot is a tiny shell script intended for updating all of your tracked dotfiles to a repository.

On first run, updot will attempt to add some commonly tracked dotfiles to your ``$XDG_CONFIG_HOME/updot/updot.conf`` for you.  

You will need to add your ``repository_root`` to the updot.conf, and you should ensure that the ``dotfiles`` array matches
the files you want to push to your repository.

###installation
Save updot.  ``chmod +x updot && mv updot /usr/local/bin``

(Assuming ``/usr/local/bin`` is in your ``$PATH``)

###configuration file
An example updot.conf

    # updot configuration file
    
    # Git repository location
    # Ex: git_repo="/home/seed419/code/linux/dotfiles"
    repository_root="/home/seed419/code/linux/dotfiles"
    
    # Tracked dotfiles
    # This is an array of dotfiles to copy to your repository
    # Ex: dotfiles=( '.bashrc' '.xinitrc' '.bash_profile' )
    dotfiles=(' .aliases .bashrc .gitconfig .i3/config .prompt .rtorrent.rc .vimrc .weechat/weechat.conf .xinitrc 
    .Xresources .config/openbox/rc.xml .config/openbox/menu.xml .xmonad/xmonad.hs .config/updot/updot.conf 
    .config/twmn/twmn.conf .dircolors .colors .git-prompt .profile .xpdfrc ')

###run it
``updot``
