# flatpak-org.sabnzbd.SABnzbd
 Flatpak for SABnzbd.

### How to build

```bash
flatpak install flathub org.freedesktop.Platform//22.08 org.freedesktop.Sdk//22.08
flatpak-builder build-dir org.sabnzbd.SABnzbd.yml
flatpak-builder --user --install --force-clean build-dir org.sabnzbd.SABnzbd.yml
flatpak run org.sabnzbd.SABnzbd.yml
```

### Issues

- Tray icon does not work
- Some Python requirements are not included as I didn't fixed the build process yet, the app still works as expected (see `python3-requirements.json.excluded`)