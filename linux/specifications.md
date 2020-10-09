# Desktop entry
```desktop
[Desktop Entry]
Version=1.0
Name=CWD Reader
Comment=Official desktop Compact Web Document format reader
TryExec=/home/dario/Apps/cwd-reader/bin/reader
Exec=/home/dario/Apps/cwd-reader/bin/reader -- %u
Icon=/home/dario/Apps/cwd-reader/assets/cwd.png
Terminal=false
StartupWMClass=CWDReader
Type=Application
Categories=Document;Web;Reader;Gtk;
MimeType=x-aplication/cwd+zip;
Keywords=cwd;reader;document;web;
X-GNOME-UsesNotifications=true
```

# Icon path

The [freedesktop.org](https://specifications.freedesktop.org/icon-theme-spec/icon-theme-spec-latest.html) standard specifies in which order and directories programs should look for icons:

- `$HOME/.icons (for backwards compatibility)`
- `$XDG_DATA_DIRS/icons`
- `/usr/share/pixmaps`

