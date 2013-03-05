#updot - the dotfile repository update utility
--------------
![Screenshot.png](http://ompldr.org/vaG50ZA)
--------------
##description
updot is a bash shell script intended for updating all of your important (and not-so-important) dotfiles to a repository.

On first ``updot -u``, updot will attempt to add some commonly tracked dotfiles to your ``$XDG_CONFIG_HOME/updot/updot.conf`` for you.

--------------

##installation
Save updot.  ``chmod +x updot && mv updot /usr/local/bin``

(Assuming ``/usr/local/bin`` is in your ``$PATH``.  ``echo $PATH`` to check) 
  
Done!

![Installation.png](http://ompldr.org/vaG50Ng)

(The extra formatting arguments are optional, only ``-u`` writes the configuration file here)

You will need to add your ``repository_root`` to the updot.conf, and you should ensure that the ``dotfiles`` array matches
the files you want to push to your repository.

--------------

##configuration file
Here's what mine looks like.  The default will be almost identical except for different files.

![Configuration.png](http://ompldr.org/vaG50Zq)

--------------

##run it!
``updot``

![Help.png](http://ompldr.org/vaG50aq)
