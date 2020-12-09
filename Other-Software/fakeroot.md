---
title: Fakeroot
parent: "Other Software"
nav_order: 2
---

# Use fakeroot
Fakeroot uses SYSV IPC by default.

WSL1 does not support SYSV IPC call.

## Ubuntu or Debian or Fedora,etc...
fakeroot-tcp is included in package.

switch to use it.
```bash
# Ubuntu/Debian
update-alternatives --set fakeroot /usr/bin/fakeroot-tcp
```
```bash
# Fedora
alternatives --config fakeroot
```

## Others (Build manually)
configure with ```--with-ipc=tcp``` and build it.