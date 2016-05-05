# Microsoft Visual Code
How to Install Microsoft Visual Code in Ubuntu

## Ubuntu

### Using Repository
```console
sudo add-apt-repository ppa:ubuntu-desktop/ubuntu-make
sudo apt-get update
sudo apt-get install ubuntu-make
```

```console
umake ide visual-studio-code
```

### Without Repository
Download .zip file from MS Visual Code Site
cd /opt
mkdir mscode
unzip file in mscode directory
```console
cd /opt/mscode
unzip ../Downloads/VSCode-linux-x64.zip
```
Create launcher
```console
sudo gedit /usr/share/applications/MSVS.desktop
```

Copy and Paste the following
```console
#!/usr/bin/env xdg-open

[Desktop Entry]
Version=1.0
Type=Application
Terminal=false
Exec=/opt/msvs/code
Name=MSVS
Icon=/opt/msvs/flurry_ios_visual_studio_2012_replacement_icon_by_flakshack-d5nnelp.png
Categories=Development
```
