deb-package-modify
==================

Make changes inside an existing deb file.

- unpacks a deb file
- creates the control file
- opens the control file in your selected editor
- after you save the control file, the deb gets repacked

See http://ubuntuforums.org/showthread.php?t=110458 
See http://ubuntuforums.org/showthread.php?t=636724

Thanks to bean1975 http://ubuntuforums.org/member.php?=58325
Thanks to Loevborg http://ubuntuforums.org/member.php?u=103957

Installation: 
-------------

    sudo cp deb-package-modify /usr/local/bin/
    sudo chmod a+x /usr/local/bin/deb-package-modify

Usage:
------

    deb-package-modify package.deb

Make changes and save, then use package.modified.deb