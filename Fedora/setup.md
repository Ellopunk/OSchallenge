# Fedora setup


## Update

`dnf update`

`reboot`

## Install "required" packages (What I require for my workflow)

 ### vim and git 

`dnf install vim`
`dnf install git`

###  visual studio

- Import Repo keys

    `sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc`

- Install repo

    `sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'`

- Pull repo info 

    `dnf check-update`

- Install visual code 

    `sudo dnf install code`

### Html5 

`dnf install -y https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-27.noarch.rpm`

`dnf install -y ffmpeg-libs`