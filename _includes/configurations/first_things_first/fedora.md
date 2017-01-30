```bash
# check for / acquire updates
$ sudo dnf check-update
$ sudo dnf upgrade
# install the useful development tools package
$ sudo dnf groupinstall "Development Tools"
# install vim
$ sudo dnf install vim
```

For Fedora, there is an **excellent** tool called [Fedy](https://folkswithhats.org/)
that I use to manage my Sublime Text installation.  The one "gotcha" with the code they
host on their website to install is that the password being asked for is the `root`
password (it comes from the `su -c`).  If you do not know the `root` password, you
should be able to replace `su -c` with `sudo su -c`.  As an example, compare the
password you would need to enter with the following commands:

```bash
# this command requires the root password
$ su -c 'ls /'
Password:
bin   dev  home  lib64       media  opt   root  sbin  sys  usr
boot  etc  lib   lost+found  mnt    proc  run   srv   tmp  var
# this command requires the password for the user
$ sudo su -c 'ls /'
[sudo] password for sven:
bin   dev  home  lib64       media  opt   root  sbin  sys  usr
boot  etc  lib   lost+found  mnt    proc  run   srv   tmp  var
```

Once `Fedy` is installed, let's install a bunch of goodies including Sublime Text:

{% include screen_shot_carousel.html name='fedy' %}
