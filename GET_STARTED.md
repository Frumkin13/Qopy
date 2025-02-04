# Get Started

The default hotkey for Qopy is Windows+V which is also the hotkey for the default clipboard manager to turn that off follow [this guide](https://github.com/0PandaDEV/Qopy/blob/main/GET_STARTED.md#disable-windowsv-for-default-clipboard-manager).

All the data of Qopy is stored inside of a SQLite database.

| Operating System | Path                                                            |
|------------------|-----------------------------------------------------------------|
| Windows          | `C:\Users\USERNAME\AppData\Roaming\net.pandadev.qopy`           |
| macOS            | `/Users/USERNAME/Library/Application Support/net.pandadev.qopy` |
| Linux            | `/home/USERNAME/.local/share/net.pandadev.qopy` |

## Disable Windows+V for default clipboard manager

<video src="https://github.com/user-attachments/assets/723f9e07-3190-46ec-9bb7-15dfc112f620" controls title="Disable Windows+V for default clipboard manager"></video>

To disable the default clipboard manager popup from windows open Command prompt and run this command

```cmd
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\System" /v AllowClipboardHistory /t REG_DWORD /d 0 /f
```

After that a restart may be reqired.
