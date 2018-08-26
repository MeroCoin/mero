Mero Core integration/staging repository
======================================


It is recommended [use the shell script](https://github.com/merocoin/meroinstall) to install a Mero Masternode on a Linux server running Ubuntu 14.04 or 16.04

***

Quick installation of the Mero daemon under linux. See detailed instructions there [build-unix.md](build-unix.md)

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/merocoin/mero.git
    cd Mero
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip merod
    sudo strip mero-cli
    sudo strip mero-tx
    cd ..

Running the daemon:

    merod

Stopping the daemon:

    mero-cli stop

Demon status:

    mero-cli getinfo
    mero-cli mnsync status

All binaries for different operating systems, you can download in the releases repository:

https://github.com/merocoin/mero/releases

P2P port: 14550, RPC port: 24550
-
