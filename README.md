# Ceph-On-Raspberry-Pi
A Ceph cluster on Raspberry Pi is an awesome way to create a RADOS home storage solution (NAS) that is highly redundant and low power usage. It’s also a low cost way to get into Ceph, which may or may not be the future of storage (software defined storage definitely is as a whole). Ceph on ARM is an interesting idea in and of itself. The CRUSH algorithm determines how to store and retrieve data by computing data storage locations. CRUSH empowers Ceph clients to communicate with OSDs directly rather than through a centralized server or broker.


# Burn
#### Flash OS images to SD cards & USB drives, safely and easily.

**https://github.com/resin-io/etcher.git**

# Installers

Refer to the downloads page for the latest pre-made installers for all supported operating systems.
# Debian and Ubuntu based Package Repository (GNU/Linux x86/x64)

    ## Add Etcher debian repository:

    echo "deb https://dl.bintray.com/resin-io/debian stable etcher" | sudo tee /etc/apt/sources.list.d/etcher.list

    Trust Bintray.com's GPG key:

    sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61

    Update and install:

    sudo apt-get update
    sudo apt-get install etcher-electron

# Uninstall

sudo apt-get remove etcher-electron
sudo rm /etc/apt/sources.list.d/etcher.list
sudo apt-get update

# Redhat (RHEL) and Fedora based Package Repository (GNU/Linux x86/x64)

    Add Etcher rpm repository:

    sudo wget https://bintray.com/resin-io/redhat/rpm -O /etc/yum.repos.d/bintray-resin-io-redhat.repo

    Update and install:

    sudo yum install -y etcher-electron

    or

    sudo dnf install -y etcher-electron

# Uninstall

sudo yum remove -y etcher-electron
sudo rm /etc/yum.repos.d/bintray-resin-io-redhat.repo
sudo yum clean all
sudo yum makecache fast

# or

sudo dnf remove -y etcher-electron
sudo rm /etc/yum.repos.d/bintray-resin-io-redhat.repo
sudo dnf clean all
sudo dnf makecache

# Solus (GNU/Linux x64)

sudo eopkg it etcher

