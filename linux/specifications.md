# Desktop entry

```desktop
[Desktop Entry]
Version=1.0
Name=CWD Reader
Comment=Official desktop Compact Web Document format reader
Exec=/cwd/path/bin/executable %f
Icon=/cwd/path/assets/cwd-reader.png
Terminal=false
StartupWMClass=CWDReader
Type=Application
Categories=Document;Web;Reader;Gtk;
MimeType=x-aplication/cwd+zip;
Keywords=cwd;reader;document;web;
X-GNOME-UsesNotifications=true
```

Save this file in `/home/dario/.local/share/applications` or `/usr/share/applications` as `cwd-reader.desktop`.

# Default application

Add a line in `/home/dario/.local/share/applications/mimeapps.list` with: `application/cwd+zip=cwd-reader.desktop`.

# MIME association

Add an XML called "cwd.xml" with this content:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<mime-info xmlns="http://www.freedesktop.org/standards/shared-mime-info">
  <mime-type type="application/cwd+zip">
    <comment>CWD format file</comment>
    <glob pattern="*.cwd"/>
  </mime-type>
</mime-info>
```

Inside the `/usr/share/mime/packages` path.

# Icon

Also add the `application-cwd+zip.svg` file inside the `/usr/share/icons/hicolor/scalable/mimetypes` path.

# Update associations

- `sudo update-mime-database /usr/share/mime/`
- `sudo gtk-update-icon-cache` and `sudo gtk-update-icon-cache /usr/share/icons/hicolor/`
