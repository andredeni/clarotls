#!/bin/sh
apt-get update -y; apt-get upgrade -y
wget https://www.openssl.org/source/openssl-1.1.1a.tar.gz
tar -zxf openssl-1.1.1a.tar.gz && cd openssl-1.1.1a
./config
make
make teste
make test
sudo mv /usr/bin/openssl ~/tmp
sudo make install
sudo ln -s /usr/local/bin/openssl /usr/bin/openssl
sudo ldconfig
openssl version
reboot
