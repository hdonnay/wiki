How
===

Base System
-----------

Major releases should be downloaded as tarballs, like gentoo stages.

Point releases should be a series of bsdiffs. Any changes to /etc
should be distributed as whole files, and notify the user if local
modifications have been made.

Kernel should have to support inotify, perhaps come with a debian kernel
by default? Or a compiled vanilla kernel?

Possibly make the whole base system an initrd? Will investigate.

use bsd-style rc or something exotic like cinit.

Package Manager
---------------

Ideally written in perl, although that may be unwise to have in the base
system (expects to be in /usr). Probably written in sh.

SQLite db of packages in /var/[distro]/packaglist.db?
 * Probably a good idea if wrapping other package managers.

/var/[distro]/[packagemanager] should be a git repository containing
folders with the names of software packages. Inside should be a file
with [version number] for a name. it should contain a url to download
the source, an option to specify premake commands (default:
./configure), an option pass make commands, and a description of the
software. below is a possible example:

    http://ftp.project.org/pub/release/latest.xz
    default
    none
    A very important piece of software that you need to survive.

In addition, if there's a [version number].patch in the folder, it will
be applied upon extraction of the tarball.
