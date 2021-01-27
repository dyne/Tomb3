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

- adopt [zenroom](https://zenroom.org) for crypto functions on keys

- adopt tc-play for crypto functions on filesystems

- support BtrFS and snapshots

- export header along with key

- desktop integration i.e udev rules to avoid usb automount

- interactive verification of tomb's executable integrity

- system to split passwords in parts (lagrange interpolation in Zenroom)

- API and docs for graphical GUIs (optional, contributed)

- use mlock(2) etc. for key creation, see [this article](https://eklitzke.org/mlock-and-mlockall)

- improve steganography with outguess

- improve creation speed with fallocate(1)
