Turkcoin integration/staging tree
================================

http://www.turkcoin.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2021 Turkcoin Developers

What is Turkcoin?
----------------

Turkcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 5 minute block targets
 - ~350k total coins

The rest is the not same as Bitcoin.
 - 20 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Turkcoin client sofware, see http://www.turkcoin.org.



### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./turkcoin-qt_test

