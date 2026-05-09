# Ubuntu_Post_Installation_Guide
This repository provides a simple guide for new users of **Ubuntu 24.04**. 

## 1. Update and Upgrade Your System
Always update your system after installation to get the latest security patches and software updates:
```
sudo apt update && sudo apt upgrade
```
You can also remove unused packages to free up space:
```
sudo apt autoremove && sudo apt autoclean
```

## 2. Install the Full Ubuntu Desktop
If you installed a minimal version of Ubuntu, you can add the full desktop environment with:
```
sudo apt install ubuntu-desktop
```
> You can see what will it install on your desktop by `apt depends ubuntu-desktop`

## 3. Enable Multimedia Support
Ubuntu cannot play some video formats by default. Install restricted media codecs:
```
sudo apt install ubuntu-restricted-extras
```

## 4. Enable Click-to-Minimize
To minimize an application by clicking its icon in the dock:
```
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'
```

## 5. Install Useful Applications
Here are some recommended apps:<br>
- **gnome-tweaks** → Extra settings and customization
  ```
  sudo apt install gnome-tweaks
  ```
- **gnome-shell-extension-manager** → Extra themes and extensions
  ```
  sudo apt install gnome-shell-extension-manager
  ```
- **vlc** → Lightweight media player that supports most formats
  ```
  sudo apt install vlc
  ```
- **LibreOffice** → Powerfull Office applications
  ```
  # For latest stable version
  sudo add-apt-repository ppa:libreoffice/ppa
  sudo apt update
  sudo apt install libreoffice
  ```
- **LaTeX** → Ultimate tool for creating professional-grade technical and scientific documents
  ```
  # To install full version (include everything)
  sudo apt install texlive-full
  ```
- **TeXstudio** → Best editor for LaTeX
  ```
  sudo apt install texstudio
  ```
- **Persian Fonts** → Here you can add Persian fonts to your Linux (Thanks to [fzerorubigd](https://github.com/fzerorubigd))
  ```
  bash -c "$(curl -fsSL https://raw.githubusercontent.com/fzerorubigd/persian-fonts-linux/master/farsifonts.sh)"
  ```
