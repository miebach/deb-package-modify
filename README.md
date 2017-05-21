deb-package-modify
==================

Make changes inside an existing deb file. 

Should work for all members of the Debian GNU/Linux family, including Ubuntu and its derivates.

- Unpacks a deb file
- Creates the control file
- Opens the control file in your selected editor
- After you save the edited control file, the deb gets repacked

See http://ubuntuforums.org/showthread.php?t=110458 

See http://ubuntuforums.org/showthread.php?t=636724

Thanks to bean1975 http://ubuntuforums.org/member.php?=58325

Thanks to Loevborg http://ubuntuforums.org/member.php?u=103957

Configuration:
--------------

Edit the file deb-package-modify after line 7 to set your preferred editor.

Installation: 
-------------

    cd /usr/local/bin/
    sudo curl -O https://raw.githubusercontent.com/miebach/deb-package-modify/master/deb-package-modify
    sudo chmod a+x /usr/local/bin/deb-package-modify

Usage:
------

Choose a deb package you want to modify and run:

    deb-package-modify package.deb

Make changes and save, then use your modified package, for example:

    sudo dpkg -i package.modified.deb
    sudo apt-get install -f
