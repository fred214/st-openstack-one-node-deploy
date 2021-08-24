# st-openstack-one-node-deploy

## Prepare
Vmware palyer need update to version 16
```
# Install Vagrant
https://www.vagrantup.com/downloads

# Install Vagrant VMware Utility
https://www.vagrantup.com/vmware/downloads

# Vagrant box link
https://app.vagrantup.com/centos/boxes/7
https://mirrors.ustc.edu.cn/centos-cloud/centos/7/vagrant/x86_64/images/

vagrant box add USER/BOX    # name from https://vagrantcloud.com/boxes/search
vagrant box add --name centos7 https://mirrors.ustc.edu.cn/centos-cloud/centos/7/vagrant/x86_64/images/CentOS-7-x86_64-Vagrant-2004_01.VMwareFusion.box   # box saveing ~\.vagrant.d
vagrant box add --name centos7 C:\tmp\CentOS-7-x86_64-Vagrant-2004_01.VMwareFusion.box

# Init
vagrant plugin expunge --reinstall
vagrant init openstack https://mirrors.ustc.edu.cn/centos-cloud/centos/7/vagrant/x86_64/images/CentOS-7-x86_64-Vagrant-2004_01.VirtualBox.box
vagrant init openstack centos7

# Add vmware to path
C:\Program Files (x86)\VMware\VMware Player
```

## Usage
```
# Start
vagrant up

# Stop
vagrant halt

```