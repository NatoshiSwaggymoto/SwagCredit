UNIX BUILD NOTES
====================

To compile SwagCredit, do this:

sudo apt-get update
sudo apt-get upgrade

sudo apt-get install git

sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev
sudo apt-get install libboost-all-dev
sudo apt-get install libcurl4-openssl-dev libevent-dev

cd ~

git clone https://github.com/NatoshiSwaggymoto/SwagCredit.git
cd SwagCredit

./autogen.sh
./configure --disable-wallet --without-gui --disable-tests --disable-bench
make

The binaries are called bitcoind and bitcoin-cli and are located in the src directory.


