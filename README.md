# LIBEVENT Configuration Environment

* The source codes are located in <https://github.com/libevent/libevent>
* Required packages (Debian and its variants) as follows
```bash
apt install autoconf libtool
```
* This repository only support the libevent version < 2.2, since it only has `Makefile` building method. 
For `>2.2`, we also need to update this repository to switch a generic Makefile to `cmake`.

## About
This repository helps to build the `libevent` package and its customized application consistently on Linux and macOS.

## `libevent` path

By default, everything will be within `/usr/local` path. It can be customized via

```bash
echo "INSTALL_LOCATION=where...." > configure/CONFIG_SITE.local
```

* Build

```bash
make init
make conf
make build
make install
```

* Others

```bash
make uninstall
make clean
make distclean
```

