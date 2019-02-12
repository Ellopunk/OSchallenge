# Application install


## [Visual Studio Code](https://code.visualstudio.com/docs/setup/linux#_rhel-fedora-and-centos-based-distributions)

1)Add repository:

`sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc`

2)Add keys 

`sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/vscode.repo'`

3)Update package cache

`sudo zypper refresh`

4)Install Visual Code

`sudo zypper install code` 
(
## [Git](https://help.github.com/articles/set-up-git/)

1) Install git:

`zypper install git'

2)Configure name and email.

`git config --global user.email "email@example.com"`

`git config --global user.name "username"`

## [SSH Keys](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

1)Follow the link above for additonal information. 

### [FireFox Video Support](https://en.opensuse.org/SDB:Firefox_MP4/H.264_Video_Support)

Also might be of assitance:
 [VLC](https://en.opensuse.org/VLC)

Full transpernecy this was done in an effort to correct my html5 issues for the Linux Academy website.

### Opera

`zypper in opera`

### nodejs

`zypper install nodejs`

``` 
The following 5 NEW packages are going to be installed:
  nodejs10 nodejs10-devel nodejs-common npm10 python

The following 2 recommended packages were automatically selected:
  npm10 python
```