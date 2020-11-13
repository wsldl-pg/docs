---
title: Fakeroot
parent: "Other Software"
nav_order: 2
---

# Use fakeroot
fakeroot is using SYSV IPC by default.

but WSL1 is not supported System V IPC call now.

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