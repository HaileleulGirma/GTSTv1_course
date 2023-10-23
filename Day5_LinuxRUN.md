sudoers file is stored in /etc/sudoers by default.
chown stands for change owner
to change the group of a file but not the owner the write the chown command without the user option `chown:root filename`

At the beginning of the permission, you can differentiate between folder/directories and files by looking at how they begin. if they begin with a `d`, then it is a directory , but if it begins with a `-` it is a file.
The difference between `sudo apt upgrade`and `sudo apt upgrade` is that the upgrade modernizes to the available version while update just re-checks its list if there are available versions ready to be upgraded to. The update should come first or the machine won't know there are newer versions available.
`sudo apt remove` and `sudo apt purge` also have some similarities as they both remove installed software, but remove only removes the installed software while purge not only removes the installed software but also the dependencies(prerequisites for that software) and any other things related to the software when it was installed.   

`sudo dpkg -i <packagename>` installs a .deb file. remember that you write the full path of the package.
`sudo dpkg -r <packagename>` removes the installed .deb file.
`sudo dpkg -p <packagename>` updates the installed package.

