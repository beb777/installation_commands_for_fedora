# installation_commands_for_fedora33
 * vivaldi
```sudo dnf install dnf-utils
sudo dnf config-manager --add-repo https://repo.vivaldi.com/archive/vivaldi-fedora.repo
sudo dnf install vivaldi-stable
```
* brave
```sudo dnf install dnf-plugins-core
sudo dnf config-manager --add-repo https://brave-browser-rpm-nightly.s3.brave.com/x86_64/
sudo rpm --import https://brave-browser-rpm-nightly.s3.brave.com/brave-core-nightly.asc
sudo dnf install brave-browser-nightly
``` 
* install vlc media player   
`sudo dnf install -y vlc`  

*install tweak gnome
`sudo dnf install -y gnome-tweak-tooly`  

*Enable RPM Fusion
```sudo rpm -Uvh http://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm   
   sudo rpm -Uvh http://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm 
```
*instal jdk java
`sudo dnf install -y java-latest-openjdk`  

* install visual studio code editor 
```sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
sudo dnf check-update
sudo dnf install -y code  
```

* .deb installation
```sudo yum install dpkg
sudo dpkg -i filename.deb
```
* .rpm installation
```sudo yum localinstall sample_file.rpm
sudo rpm –i sample_file.rpm
```
* backup and restore tools
`sudo yum install timeshift.x86_64`
* install vim 
`sudo dnf install vim-enhanced`
* tar file  installed  
  - `tar -xvf filename.tar.xz`
  - `tar xvzf filemane.tar.gz`
* to download website 
`wget -r -p https://..........`
* DNS resolver borked after upgrading Fedora 33  fixing as root user. by using three line of code

`# rm -f /etc/resolv.conf`    

  ` # ln -s /run/systemd/resolve/resolv.conf /etc/resolv.conf`  
  
   `# systemctl stop systemd-resolved.service ; systemctl disable systemd-resolved.service`

