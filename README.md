## Enable WSL
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

## Update WSL
sudo apt-get update && sudo apt-get -y upgrade

## Install ansible
sudo apt-get install -y ansible

## Add VBoxManage to PATH
echo 'export PATH="${PATH}:/mnt/c/Program Files/Oracle/VirtualBox"' >> ~/.bashrc
source ~/.bashrc

## Configure passwordless sudoers
%sudo  ALL=(ALL) NOPASSWD: ALL

## Download Fedora disk image
https://download.fedoraproject.org/pub/fedora/linux/releases/30/Cloud/x86_64/images/Fedora-Cloud-Base-30-1.2.x86_64.raw.xz
e34fb3fbbb9e3b4757952cf813da80f2dea4b0d1ca311e2017b62f0c74e376d9

