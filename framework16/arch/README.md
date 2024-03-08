# Post installation steps

## Prerequisites

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

## Devtools

```console
sudo pacman -S dotnet-sdk
```

## GUI specific steps

1. Install vscode AUR package:

```console
paru visual-studio-code-bin
```

```console
paru coolercontrol
```

## GNOME packages

```console
paru gnome-shell-extension-appindicator
```

```console
gnome-shell-extension-dash-to-dock
```

```console
paru gnome-shell-extension-freon
```

```console
flatpak install org.gnome.World.Secrets
```

## Power management

### 1. Install Power profiles daemon

```console
sudo pacman -S power-profiles-daemon
```

### 2. Copy udev rules

Copy the udev rules from etc_udev_rules_d to make power profiles daemon switch profiles automatically depending on whether connected to AC or battery.

## Entertainment

### 1. Spotify

There are two ways to install Spotify:

1. Install regular package [spotify-launcher](https://archlinux.org/packages/?name=spotify-launcher). This package manages a per-user installation in your home directory, allowing Spotify to update itself independently of pacman (similar to how Spotify self-updates on other operating systems).

2. If you prefer to manage Spotify updates with pacman, instead use the AUR package [spotify](https://aur.archlinux.org/packages/spotify/) which repackages [Spotify for Linux](https://www.spotify.com/us/download/linux/).

```console
paru spotify
```

For details see https://wiki.archlinux.org/title/Spotify

### 2. How to install Steam

First we need to make sure, [OpenGL](https://wiki.archlinux.org/title/OpenGL) and [Vulkan](https://wiki.archlinux.org/title/Vulkan) are working.

Then enable [multilib](https://wiki.archlinux.org/title/Official_repositories#multilib) repo.

Finally install Steam via pacman:

```console
sudo pacman -S steam
```
