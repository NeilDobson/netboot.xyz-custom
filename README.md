## netboot.xyz-custom

### EXPERIMENTAL

Fork me!  This repo will allow you to create custom menus within netboot.xyz.
It works by using your github user name that you input and chains to this URL:

    https://raw.githubusercontent.com/${github_user}/netboot.xyz-custom/master/custom.ipxe

Once forked, you can edit the menu as much as you want.  You can compile the iPXE image to
set the `github_user` name early on so that your Github user name is set ahead of time and
will automatically display your custom submenu on boot.  You can also set your Github user
name from the Utilities menu (**Tools:** -> **Utilities** -> **netboot.xyz tools:**) which
will cause a custom menu to appear in the main menu.

If you are new to iPXE scripting, take a look at `custom.ipxe.example` and build up from that.

----

Mount the netboot.xyz CD from the SpeedyKVM control panel and reboot the server
Enter the GitHub username in the main menu
Download the netboot.tar.gz file from http://us.mirror.devuan.org/devuan/dists/stable/main/installer-i386/current/images/netboot/ and extract it.
Make linux and initrd available in /netboot on the http server
