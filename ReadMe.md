# Tuxedo dGPU Run

This package adds a command line tool for GPU offloading and context menu entries for KDE Plasma serving the same purpose.

# Installing

## CMake

```
$ mkdir build
$ cd build
$ cmake ..
$ sudo make install
```

## Debian package

```
$ debuild
```
or
```
$ gbp buildpackage
```

Replace X.X.X with the current version number
```
$ sudo apt install ../tuxedo-dgpu-run_X.X.X_all.deb
```

# Usage

## Run a program on the descrete GPU from the terminal while being in on-demand mode:

```
$ dgpu-run <command>
```

## Run a program on the descrete GPU from KDE Plasma desktop environment:

Right click on desktop entry on the desktop or Dolphin -> "Run application with descrete GPU"

## Run a program on the descrete GPU from KDE Plasma desktop environment start menu (requires KDE Plasma >= 5.25):

Right click on menu entry -> 'Run application with descrete GPU'

or

Right click on menu entry -> 'Create "Run application with descrete GPU" menu entry'

Click the newly created menu entry "\<program name\> (GPU)"
