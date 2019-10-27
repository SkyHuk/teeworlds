Teeworlds 
=========

A retro multiplayer shooter
---------------------------

This repository is a fork of BotoX fork to put instagib into use. 
Also a bit of refactoring of the original code.

This readme is a little shorter than the original one to provide me a better overview of information I need when building it.

Originally written by Magnus Auvinen.

Building on Linux or macOS
==========================

Installing dependencies
-----------------------

    # macOS
    brew install cmake freetype sdl2


Downloading repository
----------------------

    git clone https://github.com/teeworlds/teeworlds --recurse-submodules
    cd teeworlds

    # If you already cloned the repository before, use:
    # git submodule update --init


Building
--------

* Install libsdl using ``brew install sdl2``
* Install Freetype using ``brew install freetype``
* Download and unzip [bam](https://github.com/matricks/bam/archive/v0.5.1.zip) to *teeworlds/bam*
* Compile bam using one of the ``make_<system>.sh`` scripts
* Run ``./bam/bam config``
  
## Compile
``./bam/bam conf=<config> <client server ...>``

(Optional) user ``-f`` for a forced recompile.

Options for ``config``:
```
debug - Compiles debug versions of the goal packages
release - Compiles release versions of the goal packages
```

Options for goal packages:
```
game (default)
server
client
content
masterserver
tools
```
