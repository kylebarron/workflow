# Using a PIV Card from a Linux Machine



### Install OpenSC:

See the OpenSC Github wiki on [Compiling and Installing on Unix flavors](https://github.com/OpenSC/OpenSC/wiki/Compiling-and-Installing-on-Unix-flavors). The following are the website's suggestions as of 8/8/2017.

First, we need to install dependencies.
```bash
sudo apt install pcscd libccid libpcsclite-dev libssl-dev libreadline-dev autoconf automake build-essential docbook-xsl xsltproc libtool pkg-config
```

Now to build/compile the actual program. First, download the [latest version](https://github.com/OpenSC/OpenSC/releases/latest). (Scroll to the bottom and then download the `opensc-*.tar.gz`)
```bash
cd ~/Downloads
tar xfvz opensc-*.tar.gz
cd opensc-*
./bootstrap
./configure --prefix=/usr --sysconfdir=/etc/opensc
make
sudo make install
```


### Links:
<https://pivkey.zendesk.com/hc/en-us/articles/203578629-PIVKey-on-Linux>


# Using a PIV card from macOS


### Install OpenSC

Go to the OpenSC macOS [Quick Start guide](https://github.com/OpenSC/OpenSC/wiki/macOS-Quick-Start).




