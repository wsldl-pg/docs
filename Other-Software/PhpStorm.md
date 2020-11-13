---
title: PhpStorm
grand_parent: "Other Software"
parent: "Jetbrains IDEs"
#nav_order:
---

# How to use a custom WSL distribution with PhpStorm

1. Follow the installation instructions ([here](https://github.com/yuk7/wsldl#install-with-any-rootfs)) **BUT** rename the launcher  the same as one of this
```
// Found in AppData\Roaming\JetBrains\PhpStorm{YOUR_VERSION}\options\wsl.distributions.xml
debian.exe
kali.exe
opensuse-42.exe
sles-12.exe
sles-15.exe
openSUSE-Leap-15.exe
ubuntu.exe
ubuntu1604.exe
ubuntu1804.exe
wlinux.exe
pengwin.exe
wle.exe
Arch.exe
openSUSE-Leap-15-1.exe
```

The reason for this is, all the paths for WSL executables are hard coded so even if you add a custom distribution in `wsl.distributions.xml` it will not work.

**The name of the executable is not obligatory the same as the ditribution it run !**
You can install Ubuntu with a launcher named `debian.exe` and it will work.

2. Move the executable in `C:\Users\{USER}\AppData\Local\Microsoft\WindowsApps`
3. Open or reopen Phpstorm and if all is good you can use WSL as an interpreter for PHP and nodejs

# Another solution

Another solution can be found [here](https://www.jetbrains.com/help/ruby/configuring-remote-interpreters-using-wsl.html#custom_wsl).

Note that this solution seems to not work for everyone.
