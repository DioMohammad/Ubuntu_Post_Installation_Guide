# Ubuntu_Post_Installation_Guide
This repository provides a simple guide for new users of **Ubuntu 26.04**. 

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
- **Foliate** → Read books in style! Has varies format support (Thanks to [johnfactotum](https://github.com/johnfactotum/foliate))
  ```
  sudo apt install foliate
  ```
## 6. Install Useful Gnome Extensions
- **Vitals** → A glimpse into your computer's temperature, voltage, fan speed, memory usage and CPU load. (Thanks to [corecoding](https://github.com/corecoding))
- **Blur My Shell** → Adds a blur look to different parts of the GNOME Shell, including the top panel, dash and overview. (Thanks to [aunetx](https://github.com/aunetx))
- **Clipboard Indicator** → Clipboard Manager (Thanks to [Tudmotu](https://github.com/Tudmotu))
- **Caffeine** → Disable the screensaver and auto suspend (Thanks to [eonpatapon](https://github.com/eonpatapon))
- **Bing Wallpaper** → Sync your wallpaper to today's Microsoft Bing image of the day. (Thanks to [neffo](https://github.com/neffo))
- **Apps Menu** → Add a category-based menu for apps on topbar.
- **Simple Break Reminder** → It's important to remember to take a break! (Thanks to [CastilloDel](https://github.com/CastilloDel))
- **NoteDock** → A lightweight scratchpad in the GNOME Shell top panel. Notes are stored locally. (Thanks to [joquers](https://github.com/joquers))
- **TaskDock** → A lightweight task list in the GNOME Shell top panel. (Thanks to [joquers](https://github.com/joquers))
