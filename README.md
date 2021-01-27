# Tomb v3 work in progress


## Objectives:

1. portable usage on windows and mac
2. keep consistent with the user experience in v2
3. increase the security of keys
4. backward compatibility with tombs built with v2


## Resources:

- [Feature poll](https://github.com/dyne/Tomb/issues/409)
- [Milestone on v2 repo](https://github.com/dyne/Tomb/milestone/8)

### TODO import from v2

*** [#A] integrate the zenroom for custom crypto functions
	https://decodeproject.github.io/lua-zenroom

*** [#A] study cryptsetup 2.0 and integrate it

	In particular kernel keystore functionalities

*** [#A] support BtrFS and snapshots
*** [#B] modular encryption system support

    to go beyond dm-crypt/cryptsetup

    ecryptfs, tc-play

    needs tomb marks appended at end of tombs

*** [#B] udev rules to avoid usb automount of keyplug in gnome

*** [#B] sign and verify tomb script integrity

*** [#B] analyse and show tomb entropy using libdisorder

*** [#B] use inotify on tomb
    inotify can also count when was the last time tomb was used and
    unmount it automatically after a timeout, see how much free space
    is left and warn when the space is almost finished

*** DONE [#A] system to split passwords in parts
	CLOSED: [2018-01-03 Wed 19:48]

	solved with secrets.dyne.org
	
*** DONE [#B] make a graphical tomb undertaker (gnome-druid in glade?)
	CLOSED: [2018-01-03 Wed 19:49]

	solved by gtomb and qtomb

*** use mlock(2) etc. for key creation

See https://eklitzke.org/mlock-and-mlockall

*** improve steganography with outguess

*** improve creation speed with fallocate(1)
