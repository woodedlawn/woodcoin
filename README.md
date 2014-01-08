Woodcoin integration/staging tree
================================

[insert website here]

Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2011-2013 Litecoin Developers
Copyright (c) 2014 Woodcoin Developers

What is Woodcoin?
----------------

Woodcoin is clone of litecoin, which is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.

Some differences:
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Woodcoin client sofware, see http://www.woodcoin.org.

License
-------

Woodcoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake WOODCOIN_QT_TEST=1 -o Makefile.test woodcoin-qt.pro
    make -f Makefile.test
    ./woodcoin-qt_test

