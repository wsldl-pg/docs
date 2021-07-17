---
title: "Command Line Usage"
---
# Command Line Usage
#### exe Usage
```
Usage :
    <no args>
      - Open a new shell with your default settings.

    run <command line>
      - Run the given command line in that instance. Inherit current directory.

    runp <command line (includes windows path)>
      - Run the given command line in that instance after converting its path.

    config [setting [value]]
      - `--default-user <user>`: Set the default user of this instance to <user>.
      - `--default-uid <uid>`: Set the default user uid of this instance to <uid>.
      - `--append-path <true|false>`: Switch of Append Windows PATH to $PATH
      - `--mount-drive <true|false>`: Switch of Mount drives
      - `--default-term <default|wt|flute>`: Set default type of terminal window.

    get [setting]
      - `--default-uid`: Get the default user uid in this instance.
      - `--append-path`: Get true/false status of Append Windows PATH to $PATH.
      - `--mount-drive`: Get true/false status of Mount drives.
      - `--wsl-version`: Get the version os the WSL (1/2) of this instance.
      - `--default-term`: Get Default Terminal type of this instance launcher.
      - `--lxguid`: Get WSL GUID key for this instance.

    backup [contents]
      - `--tar`: Output backup.tar to the current directory.
      - `--reg`: Output settings registry file to the current directory.

    clean
      - Uninstall that instance.

    help
      - Print this usage message.
```


### Launch instance
```cmd
>{InstanceName}.exe
[root@PC-NAME user]#
```

### Run with command line
```cmd
>{InstanceName}.exe run uname -r
4.4.0-43-Microsoft
```

### Run with command line with path translation
```cmd
>{InstanceName}.exe runp echo C:\Windows\System32\cmd.exe
/mnt/c/Windows/System32/cmd.exe
```

### Change Default User(id command required)
```cmd
>{InstanceName}.exe config --default-user user

>{InstanceName}.exe
[user@PC-NAME dir]$
```

### Set "Windows Terminal" as default terminal
```cmd
>{InstanceName}.exe config --default-term wt
```

### How to uninstall instance
```cmd
>{InstanceName}.exe clean

```


See [Hidden Options](Hidden-Options.md) for features not listed here.

It is useful for automating installation and management.
