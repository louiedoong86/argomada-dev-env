# Sublime Text 3 - Text Editor
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo add-apt-repository -y ppa:webupd8team/sublime-text-3
sudo apt-get update
sudo apt-get install sublime-text-installer
exit
```

**Install package manager in sublime text 3**

- Open Sublime text 3 and press `Ctrl ~` and paste the code below and wait for it to finish.

```
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

**Sync Sublime Text 3 to multiple machines**

- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/.config/sublime-text-3/Packages/
mkdir ~/Dropbox/Sublime
mv User ~/Dropbox/Sublime/
ln -s ~/Dropbox/Sublime/User
exit
```

Reference : [https://packagecontrol.io/docs/syncing](https://packagecontrol.io/docs/syncing)

# Htop - Process Monitor
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y htop
exit
```

# Zsh, oh-my-zsh - Shell
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y zsh
sudo apt-get install -y curl
curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh
sudo chsh -s `which zsh`
sudo reboot
atom ~/.zshrc
exit
```

- In `.zshrc` change `ZSH_THEME="ys"`.
- Restart the shell to apply configuration.

# Tmux - Terminal Multiplexer
- Open a terminal.
- Copy and paste the command below and press enter.

```
sudo apt-get install -y tmux
exit
```


# Git - Version Control
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install -y git
exit
```

**Git configuration**

- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
git config --global user.name "Firstname Lastname"
git config --global user.email firstnamelastname@gmail.com
git config --global color.ui auto
git config --global color.branch auto
git config --global color.diff auto
git config --global color.status.auto
echo 'alias glog="git log --graph --pretty=format:'\''%C(blue)%h%Creset - %C(yellow)%s%Creset %C(green)(%cr)%Creset <%aN>'\''"' >> ~/.zshrc
exit
```

# Generate SSh key - Security and ease
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
ssh-keygen -t rsa -C "firstnamelastname@gmail.com"
exit
```

- Register the generated keys to github, bitbucket, et. al.
- [https://help.github.com/articles/generating-ssh-keys](https://help.github.com/articles/generating-ssh-keys)

# TeamViewer - Remote Assistance
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/Downloads
wget http://download.teamviewer.com/download/teamviewer_linux.deb
```

- The command below will eventually fail, proceed anyway.
- Copy and paste the commands below line per line and press enter.

```
sudo dpkg -i teamviewer_linux.deb
exit
```

- Install missing dependencies.
- Open a terminal copy and paste the commands below line per line and press enter.

```
sudo apt-get install -f
sudo dpkg -i teamviewer_linux.deb
exit
```

# Virtualbox - Virtualization
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y dkms
sudo sh -c 'echo "deb http://download.virtualbox.org/virtualbox/debian trusty contrib" >> /etc/apt/sources.list.d/virtualbox.list'
wget -q http://download.virtualbox.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add -
sudo apt-get update
sudo apt-get install -y virtualbox-4.3
exit
```

# Vagrant - Virtualization wrapper
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/Downloads
wget https://dl.bintray.com/mitchellh/vagrant/vagrant_1.7.2_x86_64.deb
sudo dpkg -i vagrant_1.7.2_x86_64.deb
exit
```

# Dropbox - Cloud storage
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y nautilus-dropbox
exit
```

# Google Drive - Cloud storage
- Visit the link, [https://www.thefanclub.co.za/how-to/ubuntu-google-drive-client-grive-and-grive-tools](https://www.thefanclub.co.za/how-to/ubuntu-google-drive-client-grive-and-grive-tools)
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo add-apt-repository ppa:thefanclub/grive-tools
sudo apt-get update
sudo apt-get install grive-tools
exit
```

1. Start the application from the `dash` by searching for Grive Setup
2. Once Grive is installed, you will be asked to give Grive permission to access your Google Drive.
3. When you click Next a browser window should open and present you with Google Login page.
4. Log in to your Google Account.
5. You will then be asked to give Grive permission to access you Google Drive.
6. Click Accept to continue.
7. You will then be give a Google authentication code to copy and paste into the Grive Setup box provided.
8. Copy the code from your browser and paste in the Grive Setup box.
9. When the first sync is complete the installer will quit.
10. After installation you will find a Google Drive and Google Drive Indicator launcher icons in your Dash.
11. Click on the Google Drive Indicator to start.

# Scudcloud - Communication
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-add-repository -y ppa:rael-gc/scudcloud
sudo apt-get update
sudo apt-get install -y scudcloud
sudo apt-get install -y hunspell-en-us
exit
```

# Messenger - Communication
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd
cd Downloads
wget https://github.com/Aluxian/Facebook-Messenger-Desktop/releases/download/v1.4.0/Messenger_linux64.deb
sudo dpkg -i Mess*
exit
```

# Nodejs
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y build-essential libssl-dev curl
curl https://raw.githubusercontent.com/creationix/nvm/v0.20.0/install.sh | sh
echo "source ~/.nvm/nvm.sh" >> ~/.zshrc
exit
```

- Restart the terminal.
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
nvm ls-remote
nvm install 0.12.2
nvm alias default v0.12.2
exit
```

# Bower - Front End Package manager
- Take note that nodejs is required prior to installing bower.
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
npm install -g bower
exit
```

# Z - Directory Jumper
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~
git clone git@github.com:rupa/z.git .bin/z/
echo ". /home/`whoami`/.bin/z/z.sh" >> ~/.zshrc
exit
```

# Flash plugin for Firefox
- Go to [https://get.adobe.com/flashplayer](https://get.adobe.com/flashplayer), download the tar.gz format.
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/Downloads
gunzip install_flash_player_11_linux.x86_64.tar.gz
tar -xvf install_flash_player_11_linux.x86_64.tar
sudo cp libflashplayer.so /usr/lib/firefox/browser/plugins
exit
```

# Python 3 dependencies
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y python3-dev
exit
```

# pip3 - Python Package Manager
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/Downloads
wget https://bootstrap.pypa.io/get-pip.py
sudo python3 get-pip.py
exit
```

# Python Virtual Environment
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
pip3 install --user virtualenv
exit
```

# User Python Environment
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
~/.local/bin/virtualenv ~/penv
echo "source ~/penv/bin/activate" >> ~/.zshrc
exit
```

# Autocomplete Python Shell
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd
touch .pythonrc
echo "import rlcompleter" >> .pythonrc
echo "import readline" >> .pythonrc
echo 'readline.parse_and_bind("tab: complete")' >> .pythonrc
echo 'export PYTHONSTARTUP="$HOME/.pythonrc"' >> .zshrc
exit
```

# Python Packages
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
pip install django
pip install Pillow
pip install pep8
pip install colorama
pip install mkdocs
exit
```

- Append in atom config file, `pep8ExecutePath: /penv/path/`

# Clam AV - Anti Virus
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y clamav
sudo apt-get install -y clamav-daemon
sudo apt-get install -y libclamunrar6
exit
```

# ergo - Task viewer
- Follow instructions in the link below.
- [https://github.com/argomada/ergo](https://github.com/argomada/ergo)

# Docker - Linux containers
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
wget -qO- https://get.docker.com/ | sh
sudo docker run hello-world
sudo docker pull mysql
sudo docker pull postgres
sudo docker pull django
sudo docker pull nginx
exit
```

# SQLite3 - Database
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y  sqlite3
exit
```

# Dia - Diagramming
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y  dia
exit
```

# MySQL Client
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y  mysql-client
exit
```

# nmap - Network Mapper
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo apt-get install -y nmap
exit
```

# Synapse - Launcher
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
sudo add-apt-repository ppa:synapse-core/ppa
sudo apt-get update
sudo apt-get install -y synapse
exit
```

# Validate installation
- Open a terminal.
- Copy and paste the commands below line per line and press enter.

```
cd ~/Downloads
wget https://raw.githubusercontent.com/argomada/argomada-dev-env/master/check.py
python check.py
```

- Review this procedure if you have failed the test.
