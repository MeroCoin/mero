Mero Core version 1.2.0 is now available from:  <https://github.com/MeroCoin/mero/releases>

This is a new major version release, including various bug fixes and performance improvements, as well as updated translations.

Please report bugs using the issue tracker at github: <https://github.com/MeroCoin/mero/issues>


Mandatory Update
==============


How to Upgrade
==============

If you are running an older version, shut it down. Wait until it has completely shut down (which might take a few minutes for older versions), then run the installer (on Windows) or just copy over /Applications/mero-Qt (on Mac) or merod/mero-qt (on Linux).


Compatibility
==============

Mero Core is extensively tested on multiple operating systems using the Linux kernel, macOS 10.10+, and Windows 7 and later.

Microsoft ended support for Windows XP on [April 8th, 2014](https://www.microsoft.com/en-us/WindowsForBusiness/end-of-xp-support), No attempt is made to prevent installing or running the software on Windows XP, you can still do so at your own risk but be aware that there are known instabilities and issues. Please do not report issues about Windows XP to the issue tracker.

Apple released it's last Mountain Lion update August 13, 2015, and officially ended support on [December 14, 2015](http://news.fnal.gov/2015/10/mac-os-x-mountain-lion-10-8-end-of-life-december-14/). Mero Core software starting with v1.2.0 will no longer run on MacOS versions prior to Yosemite (10.10). Please do not report issues about MacOS versions prior to Yosemite to the issue tracker.

Mero Core should also work on most other Unix-like systems but is not frequently tested on them.

Notable Changes
==============

## GUI Changes

- Updated graphic icons

## RPC Changes

## Build System Changes
- Gitian determenistic builds working
- depends system and patches updated

### New Architectures for Depends

The depends system has new added support for the `s390x` and `ppc64el` architectures. This is done in order to support the future integration with [Snapcraft](https://www.snapcraft.io), as well as to support any developers who may use systems based on such architectures.

1.2.0 Change log
==============

Detailed release notes follow. This overview includes changes that affect behavior, not code moves, refactors and string updates. For convenience in locating the code changes and accompanying discussion, both the pull request and git merge commit are mentioned.

### Core Features
 - #3 `465c5cf` [Core] Enable enforcement so it doesnt take the whole block as POS (Dud-man)

### Build System
 - [Build] Update Depends from upstream + Gitian

### P2P Protocol and Network Code

### GUI
 - Updated graphic icons
### RPC/REST

### Wallet
 
### Miscellaneous
 - [Trivial] - add Wakie87 pgp key
## Credits

Thanks to everyone who directly contributed to this release:
Dud-man
Wakie87
royhodge