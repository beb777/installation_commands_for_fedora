# installation_commands_for_fedora
* brave
```sudo dnf install dnf-plugins-core
sudo dnf config-manager --add-repo https://brave-browser-rpm-nightly.s3.brave.com/x86_64/
sudo rpm --import https://brave-browser-rpm-nightly.s3.brave.com/brave-core-nightly.asc
sudo dnf install brave-browser-nightly```
* vivaldi
```sudo dnf install dnf-utils
sudo dnf config-manager --add-repo https://repo.vivaldi.com/archive/vivaldi-fedora.repo
sudo dnf install vivaldi-stable```
* .deb installation
```sudo yum install dpkg
sudo dpkg -i filename.deb```
* .RMP installation
```sudo rpm –i sample_file.rpm
sudo yum localinstall sample_file.rpm```
