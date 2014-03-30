autotools-demo
==============

This project should demonstrate basic usage of the GNU autotools.

## example0
The simplest configuration, only `configure.ac`.

```
autoreconf -i
./configure
```

## example1
Compile file `main.c` which includes `config.h`.

```
autoreconf -i
./configure
make
```

## example2
Compile `src/main.c`.

```
sh autogen.sh
./configure
make
```

# External build
It is also possible to build the project from other directories:

```
cd $PROJECT
mkdir example2-build
cd example2-build
../example2/configure
make
```
