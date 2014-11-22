#updot
####a colorful little dotfile repository update utility
--------------
![updot.png](https://github.com/proxa/updot/blob/master/updot.png)

##description
updot is a script for tracking and updating all of your dotfiles to your repository.

Instead copying dotfiles one by one and forgetting what files have changed, 
they are stored in updot's dotfiles array and diffed/updated automagically!

##installation
1. Save updot.  Then, ``chmod +x updot && mv updot /usr/local/bin``
(Assuming ``/usr/local/bin`` is in your ``$PATH``. You can do ``echo $PATH`` if you're not sure..)
  
2. Run ``updot -c -u`` to write your new configuration file (*-c specifies to use colors*)

3. Add your ``repository_root`` to the updot.conf, and customize your ``dotfiles`` array.

4. **Profit!**  Run ``updot -u`` and never worry about updating your dotfile repo again.

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
