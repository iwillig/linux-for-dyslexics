# Linux for Dyslexics

This script is designed to transform a fresh Fedora Linux installation
into a system that is kind to people with dyslexia.

This tool is based on the Gnome 3 Desktop and makes heavy use of the
[OpenDyslexic](https://opendyslexic.org/) Font.

This project was inspired by [Omakub](https://omakub.org/)

## Packages

This is a list of packages that I have found helpful.


1. [Fish shell](https://fishshell.com/)

```shell
# dnf install fish
```

2. [GNU Aspell](http://aspell.net/)

```shell
# sudo dnf install aspell aspell-en
```

3. [GNU Stow](https://www.gnu.org/software/stow/)

```shell
# dnf install stow
```

4. nerd-fonts

```shell
# dnf copr enable che/nerd-fonts
# dnf install nerd-fonts
```

5. [GNU Emacs](https://www.gnu.org/software/emacs/)

```shell
# dnf install emacs
```

6.  pipx

```
# sudo dnf install pipx
```

7. gnome-extensions-cli

```shell
# pipx install gnome-extensions-cli --system-site-packages
# sudo dnf install libgtop2-devel lm_sensors
```

8. gnome-extensions-cli

```shell
gext install tactile@lundal.io
gext install just-perfection-desktop@just-perfection
gext install blur-my-shell@aunetx
gext install space-bar@luchrioh
gext install undecorate@sun.wxg@gmail.com
gext install Vitals@CoreCoding.com
gext install AlphabeticalAppGrid@stuarthayhurst

gext install picture-of-the-day@swsnr.de

gext install readingstrip@lupantano.gihthub
gext install colortint@matt.serverus.co.ukn
gext install gnomebedtime@ionutbortis.gmail.com
```

9. Themes

```shell
gsettings set org.gnome.desktop.interface color-scheme 'prefer-dark'
```

10. Speech to text

```shell
flatpak install flathub net.mkiol.SpeechNote
```

11. Disable animations

```shell
gsettings set org.gnome.desktop.interface enable-animations false
```

## Common command lines tools

```shell
# sudo dnf install fzf ripgrep bat eza zoxide plocate btop apache2-utils fd-find tldr
```

## List all of the user install packages

```shell
dnf repoquery --userinstalled
```
