Djoshcoin integration/staging tree
================================


Copyright (c) 2009-2014 Bitcoin Developers

Copyright (c) 2011-2014 Litecoin Developers

Copyright (c) 2018      Djoshcoin Developers

I want to be clear that Djoshcoin is not meant to be an premine. To mine this coin right now, you should clone the repository, 
build it and run setgenerate true.

Please add your node to the node list as an pull request.


What is Djoshcoin?
----------------

Djoshcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 30 second block targets
 - subsidy halves in 4.2M blocks (~4 years)
 - ~21 million total coins
 - 2.5 coins per block
 - 120 blocks to retarget difficulty
 
 
ports:

Default:4233, Testnet:14233
Defaultrpc:4232 , Testnetrpc:14232



Dependencies
----------------

```
  sudo apt-get install git

  sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils

  sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev

  sudo apt-get install libboost-all-dev

  sudo apt-get install software-properties-common

  sudo add-apt-repository ppa:bitcoin/bitcoin

  sudo apt-get update

  sudo apt-get install libdb4.8-dev libdb4.8++-dev

  sudo apt-get install libminiupnpc-dev

  sudo apt-get install libzmq3-dev

  sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler

  sudo apt-get install libqt4-dev libprotobuf-dev protobuf-compiler
```

Building:
----------------
```
  cd src/
  make -f makefile.unix		# Headless Djoshcoin
```

See readme-qt.rst for instructions on building Djoshcoin-Qt, the graphical user interface.

In your djoshcoin.conf file add
```
  addnode=136.144.168.39
```


Roadmap
----------------

- Create an block explorer
- Create an mining pool
- Add Djoshcoin to an exchange
- Let the community run the project


