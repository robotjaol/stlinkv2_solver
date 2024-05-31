## Upgrade Frimware ST-LINK

This package contains the installer for USB ST-Link probe related .rules files.
It will install in directory /etc/udev/rules.d/ the following files:
49-stlinkv2-1.rules 49-stlinkv2.rules 49-stlinkv3.rules and 49-stlinkv1.rules.
Note that a file is provided for ST-Link/V1 despite most toolsets do not support it.

To install st-stlink-udev-rules for Linux on your system use one of the package provided.
The package to use depends on your machine distribution but also on your system knowledge.

1. Go To **stlink** directory

2. Go To **AllPlatforms** directory

3. Go To **StlinkRulesFilesForLinux** directory

4. Then Type this command 

    ```
    sudo dpkg -i ./st-stlink-udev-rules-1.0.3-2-linux-all.deb

    ```
5. And run ``sudo apt update``

6. Debug Your STM32 

---

### Another OS installation

* RPM-based distribution (Redhat, Centos, Suse, Fedora...)
    As root user:
    - either run: sudo rpm -Uhv st-stlink-udev-rules-xxxx-linux-noarch.rpm
    - or use the dedicated software package manager from your system
    
* Debian-based distribution (Debian, Ubuntu...)
    As root user:
    - either run: ``sudo dpkg -i st-stlink-udev-rules-xxxx-linux-all.deb``
    - or use the dedicated software package manager from your system

* Any/other distribution (but prefer one of the native method above if you can)
    As root user
    - run: ``sudo sh st-stlink-udev-rules-xxxx-linux-noarch.sh``
