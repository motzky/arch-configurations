# Post installation steps

1. Development tools

```console
sudo pacman -S --needed base-devel
```

```console
rustup default stable
```

2. Clone & Install [PARU](https://github.com/Morganamilo/paru)

```console
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si
```

# Devtools

```console
sudo pacman -S dotnet-sdk
```

# GUI specific steps

1. Install vscode AUR package:

```console
paru visual-studio-code-bin
```

```console
paru coolercontrol
```

```console
paru spotify
```

# GNOME packages

```console
paru gnome-shell-extension-appindicator
```

```console
gnome-shell-extension-dash-to-dock
```

```console
paru gnome-shell-extension-freon
```
