## BEWARE: This doesn't really work with the default Ubuntu LTS installer in 24.04. The primary problem is that the flutter-based installer can't handle installing to pre-existing LVM volumes! If they ever fix that glaring oversight, this script may again be of some use.

# LUKS-guided-manual-partitioning
Easily install Ubuntu with FDE and semi-manual partitioning see the full write-up [here](https://adventures-in-tech.blogspot.com/2018/10/encrypted-ubuntu-installation-with.html)

In short, LGMP enables you to set up an encrypted Ubuntu installation with semi-manual partitioning. In fact, if you know what you're doing, you could very easily set up additional logical volumes during the installation process.
In addition, LGMP creates some useful scripts on the desktop that can be used to change the encryption passphrase or recover from a forgotten passphrase, recover from corrupted LUKS headers, and reinstall to the same encrypted setup, keeping /home intact.

Simply copy the LGMP.sh script to a system running a Live Ubuntu OS from USB or DVD, and run it. It will walk you through the process step-by-step. Have multiple disks and you want to install to /dev/sdb? No problem. The script can handle that.

This script has been tested on the following Ubuntu OSs:
  * 18.04
  * 20.04
