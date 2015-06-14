# Download Ubuntu OS
- Click the link below.
- [http://releases.ubuntu.com/14.04.2/ubuntu-14.04.2-desktop-amd64.iso.torrent](http://releases.ubuntu.com/14.04.2/ubuntu-14.04.2-desktop-amd64.iso.torrent)
- Using a torrent client open and download the torrent file.

# Prepare the flash drive
- Secure a 2GB or greater capacity flash drive.
- Format the flash drive using FAT32 file system.
- Insert the flash drive to the computer.

# Download and install unetbootin

**For Ubuntu**

- Open a terminal copy and paste the command and press enter.

    ```
    sudo apt-get install -y unetbootin
    ```

**For Windows**

- Click the link below and wait for the download to finish.
- [http://unetbootin.sourceforge.net/unetbootin-windows-latest.exe](http://unetbootin.sourceforge.net/unetbootin-windows-latest.exe)

# Make the flash drive bootable
- Click or execute unetbootin.
- Select disk image.
- Press `...` button.
- Find and click the Ubuntu OS image.
- Press Open button in the dialog box.
- Click Ok button in unetbootin.
- Wait for the process to complete.
- Reboot when prompted.

# BIOS configuration
- Enter BIOS mode before the previous OS will boot.
- Ensure USB boot feature is enabled in BIOS.
- Ensure EUFI feature in boot is enabled in BIOS.
- Save the changes and reboot.

# After booting
- Select live mode in the bootloader menu.
- Wait for ubuntu to load competely
- Test all peripheral devices are working.
- Click install icon found in the desktop.

# Ubuntu OS installation

**Delete and Partition Disk**

- In `dash` type gparted and click gparted.
- Delete previous partitions in the disk using gparted.
- Ensure only one partition on the disk in gparted.
- Use the references below to install ubuntu.
- Commit to settings and install.
- Restart if prompted.

# References
- [http://www.ubuntu.com/download/desktop/install-ubuntu-desktop](http://www.ubuntu.com/download/desktop/install-ubuntu-desktop)
- [http://www.wikihow.com/Install-Ubuntu-Linux](http://www.wikihow.com/Install-Ubuntu-Linux)
- [http://www.dedoimedo.com/computers/gparted.html](http://www.dedoimedo.com/computers/gparted.html)
- [http://www.everydaylinuxuser.com/2014/05/install-ubuntu-1404-alongside-windows.html](http://www.everydaylinuxuser.com/2014/05/install-ubuntu-1404-alongside-windows.html)

# Programming font
- Open in a new tab [http://programmingfonts.org](http://programmingfonts.org)
- Download and install programming font of choice.

# Update and upgrade
- Open a terminal
- Copy and paste the command below and press enter.

```
sudo apt-get update && sudo apt-get upgrade -y && exit
```

# Linux commandline commands
**Open the following links below and study.**

- [https://help.ubuntu.com/community/UsingTheTerminal](https://help.ubuntu.com/community/UsingTheTerminal)
- [http://cli.learncodethehardway.org/book](http://cli.learncodethehardway.org/book)
- [http://linuxcommand.org](http://linuxcommand.org)
- [http://ss64.com/bash](http://ss64.com/bash)
- [http://www.commandlinefu.com](http://www.commandlinefu.com)
- [http://www.ee.surrey.ac.uk/Teaching/Unix](http://www.ee.surrey.ac.uk/Teaching/Unix)
- [http://ryanstutorials.net/linuxtutorial/commandline.php](http://www.ee.surrey.ac.uk/Teaching/Unix)
