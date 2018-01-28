# slack-kernel-hook

Automate configuring initrd and bootloader on Slackware linux.

I use this for automating kernel upgrades with
[slackroll](https://github.com/rg3/slackroll)

    # slackroll batch kernel-upgrade
    # slack-kernel-hook --vtcol
    # reboot
    # slackroll batch clean-kernel
    # slack-kernel-hook --vtcol

If you have installed [vtcol](https://github.com/phi-gamma/vtcol) (available
on slackbuilds.org), you can have it automatically added to your initrd.

If you have installed [early-ssh](http://dev.kakaopor.hu/early-ssh/) (available
on slackbuilds.org), you can have it automatically added to your initrd.

The script supports lilo and grub, though lilo is less well tested since I
usually use grub.
