```bash
sudo pacman -S fish
```

```bash
sudo pacman -S xdg-desktop-portal-hyprland xdg-desktop-portal-gtk hyprpicker wl-clipboard cliphist inotify-tools app2unit wireplumber trash-cli foot fish fastfetch starship btop jq eza adw-gtk-theme papirus-icon-theme qt5ct-kde qt6ct-kde ttf-jetbrains-mono-nerd
```

```bash
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

```bash
yay -S quickshell-git
```

```bash
git clone https://github.com/caelestia-dots/caelestia.git ~/.local/share/caelestia
git clone https://github.com/caelestia-dots/shell.git ~/.local/share/caelestia-shell
fish install.fish --noconfirm

```

```
caelestia shell -d
```

Настрой файл конфигов `~/.config/caelestia/shell.json` для тонкой настройки визуала, тем, иконок и поведения интерфейса

Убедись, что остальные конфиги (Hyprland, терминал, fish, btop и др.) правильно расположены в `~/.config` (либо через symlinks) как задаёт скрипт установки
