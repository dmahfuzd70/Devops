Installing VirtualBox from Oracle repositories

Follow the steps below to install the VirtualBox on your CentOS 7 machine:

    Start by downloading the build tools necessary for compiling the vboxdrv kernel module:

    sudo yum install kernel-devel kernel-headers make patch gcc

    Copy

    Download the Oracle Linux repo file to /etc/yum.repos.d directory using the following wget command:

    sudo wget https://download.virtualbox.org/virtualbox/rpm/el/virtualbox.repo -P /etc/yum.repos.d

    Copy

    Install the latest version of VirtualBox 5.2.x by typing:

    sudo yum install VirtualBox-5.2

    Copy

    During the installation, you will be prompted to import repository the GPG key. Type y and hit Enter. Once the installation is complete you will see the following output:

    Creating group 'vboxusers'. VM users must be member of that group!

    Verifying  : VirtualBox-5.2-5.2.20_125813_el7-1.x86_64

    Installed:
    VirtualBox-5.2.x86_64 0:5.2.20_125813_el7-1

    Copy

    To verify that your VirtualBox installation was successful, run the following command which will check the status of the vboxdrv service.

    systemctl status vboxdrv

    Copy

    The output should look something like this indicating that the service is enabled and active :

    ● vboxdrv.service - VirtualBox Linux kernel module
        Loaded: loaded (/usr/lib/virtualbox/vboxdrv.sh; enabled; vendor preset: disabled)
        Active: active (exited) since Thu 2018-10-25 21:31:52 UTC; 6s ago
