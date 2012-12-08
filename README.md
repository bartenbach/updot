#updot
--------------

###description
updot is a tiny shell script intended for updating all of your tracked dotfiles to a repository.

At the moment, the only command available is just ``updot``.  On first run, updot will attempt to add commonly tracked dotfiles
to your ``$XDG_CONFIG_HOME/updot/updot.conf`` for you.  Of course, you will have to edit the updot config file after first run to 
add your repositories root folder anyway, so it's probably also a good time to verify that the dotfiles array is correct, and add/remove 
other dotfiles to your liking.

###installation
Save the updot file somewhere.  cd to its directory.  ``chmod +x updot && mv updot /usr/local/bin``

Of course, really updot doesn't *have* to be in ``/usr/local/bin``.  It can reside in any directory in your ``$PATH``

###configuration file
This is my personal configuration file, which is reflected by my dotfiles repository:

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
