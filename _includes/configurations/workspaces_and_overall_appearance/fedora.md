## Install `gnome-tweak-tool` and Download Workspace Grid
----------------------------------------------------------------------------------------

**Note**: I run (and release VMs of) Fedora with the **Gnome** desktop manager.  If you
are not using **Gnome** with Fedora (e.g. you selected KDE), this will not work.  On the
other hand, if you are using a different flavor of Linux that has **Gnome** installed,
you _can_ follow these instructions!

```bash
# install the _excellent_ gnome tweak tool
$ sudo dnf install gnome-tweak-tool
# determine which version of gnome we are running
$ gnome-shell --version
```

Now that we have `gnome-tweak-tool`, we can install "Extensions".  The extension we will
install is called [Workspace Grid][workspace_grid_home].  Visit the
[workspace grid downloads page][workspace_grid_down], and download the `.zip` that
claims support for the output of `gnome-shell --version`.  For example, in the Fedora 25
VM, at the time of installation we were running `GNOME Shell 3.22.2`, and the latest
release

[workspace_grid_home]: https://github.com/zakkak/workspace-grid-gnome-shell-extension
[workspace_grid_down]: https://github.com/zakkak/workspace-grid-gnome-shell-extension/releases

## Go Dark, Setup Workspaces, and More With `gnome-tweak-tool`
----------------------------------------------------------------------------------------

{% include screen_shot_carousel.html name='tweak_and_workspace_grid' %}



