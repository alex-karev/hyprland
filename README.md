# My [Hyprland](https://hyprland.org/) config

## Screenshots

<img src="https://github.com/alex-karev/hyprland/raw/main/screenshots/screenshot1.png">

<img src="https://github.com/alex-karev/hyprland/raw/main/screenshots/screenshot2.png">

## Description

A hyprland+waybar+wofi+dunst config inspired by my custom dwm build: [dwm](https://github.com/alex-karev/dwm).

## Features
* Stylized waybar.
* Stylized wofi launcher.
* [Catppuccin](https://github.com/catppuccin/catppuccin) theme.
* Window rules for associating windows with workspaces.
* HIDPI support.
* Multimonitor support.
* Scripts for changing volume and brightness using dunst.
* Screenshot pipeline via slurp+grim+swappy.

## Installation
1. Install dependencies:

```
sudo pacman -S hyprland hyprpaper hyprlock waybar dunst brightnessctl pamixer slurp swappy grim kitty
yay -S catppuccin-cursors-mocha catppuccin-gtk-theme-mocha
```

2. Clone this repo:

```
git clone https://github.com/alex-karev/hyprland.git
cd hyprland
```

3. Make scripts in ```scripts``` directory executable and copy them to ```/usr/local/bin``` *(or wherever you store your scripts)*:

```
chmod +x scripts/*
cp scripts/* /usr/local/bin/
```

4. Link dotfiles
```
ln -s $(pwd)/config/hypr $HOME/.config/hypr
ln -s $(pwd)/config/waybar $HOME/.config/waybar
ln -s $(pwd)/config/dunst $HOME/.config/dunst
ln -s $(pwd)/config/wofi $HOME/.config/wofi
```

## Configuration

You can edit everything in `config` directory.

> Wallpaper from screenshots: [wallhaven.cc](https://wallhaven.cc/w/p9zjrj)
