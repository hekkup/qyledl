# qyledl #

http://hekkup.github.com/qyledl/

This is a GUI for [yle-dl](http://aajanki.github.com/yle-dl/index.html) for downloading media clips from [YLE Areena](http://areena.yle.fi/).

The GUI is written in C++/[Qt](http://qt-project.org/) and currently requires yle-dl installed.

qyledl is based on [mpartel's yle-downloader-gui](https://github.com/mpartel/yle-downloader-gui).

Snapshot packages for Ubuntu are available from https://launchpad.net/~hekkup/+archive/yle-downloader-gui-snapshots.

See below for instructions for installation in Windows.

## Compiling ##

- `lrelease yle-downloader-gui.pro`
- `qmake`
- `make`

### Running Tests ###

- `cd test`
- `qmake`
- `make all check`

## Installation in Linux ##

In order to install the application in Linux run the following command. If it doesn't work, please check the installation paths of files in `yle-downloader-gui.pro` project file. The file paths have been tested on Kubuntu 13.04 and they should be more or less the same in other distributions, too.

- `sudo make install`

Uninstallation:

- `sudo make uninstall`

## Installation in Windows ##

An installation package for Windows is available at http://mpartel.github.io/yle-downloader-gui/

Instructions for generating a precompiled installation package for Windows are available at https://github.com/mpartel/yle-downloader-gui#yle-areena-downloader-gui


## Known Issues ##

- On Windows, when trying to download a file that already exists, yle-dl crashes to an encoding error while printing a log message.

## Thanks ##

- [Antti Ajanki](https://github.com/aajanki) for yle-dl
- [Martin Pärtel](https://github.com/mpartel) for yle-downloader-gui (the base for qyledl)
- [Jesse Jaara](https://github.com/Huulivoide) for a better icon and suggestions
- [Tomas Strand](https://github.com/straend) for YLE Passi support (back when it existed)

## Version History ##

- 2.3 (2013-11-05)
    * New fork: qyledl
    * Version numbering continued directly from yle-downloader-gui
    * Added download queue, support for English, etc.

- 2.2 (2013-02-21)
    * Updated yle-dl to 2.0.2.
    * Accept a URL as a command line parameter.

- 2.1 (2012-06-07)
    * Updated yle-dl to 1.99.8.
    * Added ability to give command line options in the URL box.
    * Added options to download swh and eng subtitles.

- 2.0 (2012-05-28)
    * Updated yle-dl to 1.99.7.

- 1.99.1 (2012-04-24)
    * Updated yle-dl to 1.99.6.
    * Added subtitle selection box.

- 1.99 (2012-04-17)
    * Support for Areena Beta.

- 1.3 (2012-01-02)
    * Added support for YLE Passi.

- 1.2 (2011-12-05)
    * Updated rtmpdump-yle to 1.4.6, which fixed some Areena downloads.

- 1.1 (2011-10-11)
    * Updated rtmpdump-yle to 1.4.4, which fixed Elävä Arkisto and YleX on Windows.
    * Passed the `--vfat` switch on Windows.

## License ##

Public Domain, but note that yle-dl is under GPLv2, so treat this as GPL'ed too if you like.
