slim-pkg-config
===============

Lightweight alternative to pkg-config with significant speed up for large projects. 

author: Erik Rodner (Erik dot Rodner at gmail.com)

I wrote this pkg-config alternative basically for the nice-core library, which uses an own make/pkg-config build system. In this project every directory is a library itself and dependencies are implicitly defined using the directory structure. This generates a long list of depending .pc files. The original pkg-config script expands the command arguments immediately without considering duplicate entries, which causes a long command line and a bad performance. My slim-pkg-config script works differently and first eliminates duplicate entries.

Please note that slim-pkg-config only offers the basic functionality of pkg-config.
