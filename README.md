opencpn-sglock PPA Readme
=========================

This PPA contains a library which is necessary for using the 
hardware dongle supported by the opencpn o-charts plugin [1]

The PPA is targeting Debian users. Using Ubuntu PPAs is in general not
recommended on Debian. However, this PPA has very few dependencies and 
should be fine to use also on Debian.

The PPA is available at
https://launchpad.net/~leamas-alec/+archive/ubuntu/opencpn-sglock

Usage 
-----

Initialize the PPA on Debian: 

    $ sudo add-apt-repository \
       'deb https://ppa.launchpadcontent.net/leamas-alec/opencpn-sglock/ubuntu/ noble main'
    $ sudo apt update

Install on an arm64/aarch64 host:

    $ sudo apt install opencpn-sglock-arm64

Install on an amd64/x86_64 host:

    $ sudo apt install opencpn-sglock-amd64

Build info
----------

Building packages:

    $ cd amd64
    $ make orig
    $ debuild -S

    $ cd ../arm64
    $ make orig
    $ debuild -S


[1] https://opencpn.org/OpenCPN/plugins/ocharts.html
