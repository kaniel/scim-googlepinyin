

# Introduction #

This document is intended to help you to build and install scim-googlepinyin from scratch.

# grab the source #

Scim-googlepinyin still has some critical bugs. And it is still under active development. I'd like to suggest you always try the latest version by:
```
 $ git clone git://github.com/tchaikov/scim-googlepinyin.git
 $ cd scim-googlepinyin.git
```
If the `git` command is not available in your system, you may want to install it to continue checking out the source.

# build depends #

You will need install following package before building this software:

  * automake
  * libtool
  * autotools-dev
  * libgtk2.0-dev
  * libscim-dev

Although these packages' names vary, they are available on most GNU/Linux distribution. On Debian or Ubuntu, following command should work for you.
```
 $ aptitude install autotools-dev libgtk2.0-dev libscim-dev
```

# runtime depends #
  * scim

# build and install #
Following commands installs scim-googlepinyin into your system.
```
 $ ./autogen.sh
 $ make
 $ sudo make install
```