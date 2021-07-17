---
title: "Hidden Options"
---
These are commands for distribution developers, so there is no need for documentation.
# Hidden Options
## Common
### version
```cmd
>{InstanceName}.exe version
wsldl2, version 21071600  (amd64)
https://git.io/wsldl
```
### isregd
```cmd
>{InstanceName}.exe isregd
>echo %ERRORLEVEL%
0
```
Returns 0 if registered instance.

## Install
### Install Option (Silent)
1. Install Only
```cmd
>{InstanceName}.exe install
```

2. with tarball
```cmd
>{InstanceName}.exe install {fileName}
```

3. MS Compatibility (root mode install/silent)
```cmd
>{InstanceName}.exe install --root
```

## Installed
### Run with arg
`{InstanceName}.exe -c {commands}` and `{InstanceName}.exe /c {commands}` for MS launcher compatibility.
### Silent Cleanup
```cmd
>{InstanceName}.exe clean -y
```
