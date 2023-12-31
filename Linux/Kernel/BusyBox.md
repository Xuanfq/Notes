
# BusyBox

## What is busybox:

  BusyBox combines tiny versions of many common UNIX utilities into a single
  small executable.  It provides minimalist replacements for most of the
  utilities you usually find in bzip2, coreutils, dhcp, diffutils, e2fsprogs,
  file, findutils, gawk, grep, inetutils, less, modutils, net-tools, procps,
  sed, shadow, sysklogd, sysvinit, tar, util-linux, and vim.  The utilities
  in BusyBox often have fewer options than their full-featured cousins;
  however, the options that are included provide the expected functionality
  and behave very much like their larger counterparts.

  BusyBox has been written with size-optimization and limited resources in
  mind, both to produce small binaries and to reduce run-time memory usage.
  Busybox is also extremely modular so you can easily include or exclude
  commands (or features) at compile time.  This makes it easy to customize
  embedded systems; to create a working system, just add /dev, /etc, and a
  Linux kernel.  Busybox (usually together with uClibc) has also been used as
  a component of "thin client" desktop systems, live-CD distributions, rescue
  disks, installers, and so on.

  BusyBox provides a fairly complete POSIX environment for any small system,
  both embedded environments and more full featured systems concerned about
  space.  Busybox is slowly working towards implementing the full Single Unix
  Specification V3 (http://www.opengroup.org/onlinepubs/009695399/), but isn't
  there yet (and for size reasons will probably support at most UTF-8 for
  internationalization).  We are also interested in passing the Linux Test
  Project (http://ltp.sourceforge.net).


## Link

[BusyBox](https://www.busybox.net/)


## Source Code Compile

1. Download: `wget https://www.busybox.net/downloads/busybox-1.36.1.tar.bz2`


2. Make Config: `make menuconfig`. You can do the compile options here, such as 'Settings' -> 'Build static binary (no shared libs)' -> select(y).


3. Make Install: `make install`, result is in `_install` directory.










