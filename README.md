Bitcore Node Safe
============

A Safe full node for building applications and services with Node.js. A node is extensible and can be configured to run additional services. At the minimum a node has an interface to [Safe Core v7.2.x](https://github.com/gordon87github/bitcore-safe) for more advanced address queries. Additional services can be enabled to make a node more useful such as exposing new APIs, running a block explorer and wallet service.

## Install

```bash
npm install -g bitcore-node-safe
```

## Prerequisites

- Safe Core (v0.12.1.x) with support for additional indexing *(see above)*
- Node.js v0.10, v0.12, v4 or v5
- ZeroMQ *(libzmq3-dev for Ubuntu/Debian or zeromq on OSX)*
- ~20GB of disk storage
- ~1GB of RAM

## Configuration

Bitcore includes a Command Line Interface (CLI) for managing, configuring and interfacing with your Bitcore Node.

```bash
bitcore-node-safe create -d <safe-data-dir> mynode
cd mynode
bitcore-node-safe install <service>
bitcore-node-safe install https://github.com/yourname/helloworld
bitcore-node-safe start
```

This will create a directory with configuration files for your node and install the necessary dependencies.

Please note that [Safe Core v7.2.x](https://github.com/gordon87github/bitcore-safe)  will be downloaded automatically. Once completed the safed binary should be placed into the &lt;safe-data-dir&gt; folder specified during node creation.

For more information about (and developing) services, please see the [Service Documentation](docs/services.md).

## Add-on Services

There are several add-on services available to extend the functionality of Bitcore:

- [Insight API]  npm install bitcore-api-safe
- [Insight UI]   npm install bitcore-ui-safe
- [Insight Service]npm install bitcore-node-safe
- [Insight lib]npm install bitcore-lib-safe

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/bitpay/bitcore/blob/master/CONTRIBUTING.md) file.

installation
============

## nodejs

- wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
- download nodejs version controller
- nvm install 4.6.1
- Best version  4.6.1
- Do not exceed version 4.9

## npm
sudo apt-get update
npm install npm

## libzmq
git clone https://github.com/zeromq/libzmq


rely on：
- sudo apt-get install libtool
- sudo apt-get install autoconf
- sudo apt-get install pkg-config

Execute a command 
- 1) ./autogen.sh && ./configure && make -j 4
- 2) npm config set unsafe-perm true
- 3) sudo make check && make install && sudo ldconfig
- 4) npm install -g zmq

## Node program

- sudo apt-get install libboost-all-dev
- sudo apt-get install libdb++-dev
- sudo apt-get install libminiupnpc-dev
- sudo apt-get install libevent-dev

