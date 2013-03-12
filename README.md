#updot - the dotfile repository update utility
--------------
![Screenshot.png](http://ompldr.org/vaG50bg)

##description
updot is a bash shell script intended for updating all of your important (and not-so-important) dotfiles to a repository.

On first ``updot -u``, updot will attempt to add some commonly tracked dotfiles to your ``$XDG_CONFIG_HOME/updot/updot.conf`` for you.

##installation
Save updot.  ``chmod +x updot && mv updot /usr/local/bin``

(Assuming ``/usr/local/bin`` is in your ``$PATH``. You can do ``echo $PATH`` to check) 
  
Done!

![Installation.png](http://ompldr.org/vaG50bw)

You will need to add your ``repository_root`` to the updot.conf, and you should ensure that the ``dotfiles`` array matches
the files you want to push to your repository.

##configuration file
    #
    # updot.conf - updot configuration file
    #
    
    # Repository's root folder location
    # Ex: repository_root="$HOME/code/linux/dotfiles"
    repository_root=""
    
    # Tracked dotfiles
    # This is an array of dotfiles in your $HOME to copy to your root_repository
    # Ex: dotfiles=(' .bash_profile .bashrc .inputrc .mutt/muttrc .xinitrc ')
    dotfiles=(' .bash_profile
                .bashrc
                .vimrc
                .xinitrc
                .Xresources
                .xmonad/xmonad.hs
                .inputrc
                .mutt/muttrc ')
    
    # Use color in output. true/false
    color="false"
    
    # Use bold print in output
    bold="false"
    
    # Use high intensity color in output
    high_intensity="false"
    
    # Use underlined text in output
    underline="false"
    
    # vim: set ft=sh ts=2 sw=2 et:
