# MIME association

Add an XML called `cwd.xml` with this content:

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
- `sudo gtk-update-icon-cache`
- `sudo gtk-update-icon-cache /usr/share/icons/hicolor/`
