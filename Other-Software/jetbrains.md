---
title: "Jetbrains IDEs"
parent: "Other Software"
has_children: true
nav_order: 4
---

# Jetbrains IDEs
You can use `wsl.distributions.xml` file to configure Jetbrains IDEs interpreter.

`config\options\wsl.distributions.xml`

Example:
```xml
<descriptor>
    <id>Arch</id>
    <microsoft-id>Arch</microsoft-id>
    <executable-path>c:/linux/arch.exe</executable-path>
    <presentable-name>Arch</presentable-name>
</descriptor>
```

For more details, check the link below.

https://www.jetbrains.com/help/pycharm/using-wsl-as-a-remote-interpreter.html#custom-distribution
