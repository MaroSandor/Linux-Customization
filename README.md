
# Parancsok és lépések

[YouTube Link](https://www.youtube.com/watch?v=DMs7DX3Um9E)

## 1. Rendszer-frissítés
```bash
sudo pacman -Syu
```

## 2. Nautilus fájlkezelő telepítése
```bash
sudo pacman -S nautilus nautilus-admin
```
**Preferred Applications**: File Manager > Files

## 3. Flatpak, Git, Curl, Rsync telepítése
```bash
sudo pacman -S flatpak git curl rsync
```

## 4. Asztali ikonok letiltása
**Desktop**: Desktop layout > "No desktop icons"

## 5. Új ablakok központosítása
**Windows (Behavior)**: Location of newly opened windows > "Center"

## 6. Erőforrásfájlok letöltése

### 6.1 GTK téma telepítése
```bash
unzip ~/Downloads/cinnamon-theme.zip -d ~/Downloads/
rsync -av ~/Downloads/cinnamon_theme/.themes ~
ls -al ~/.themes
```

### 6.2 Ikon téma telepítése
```bash
unzip ~/Downloads/icons-theme.zip -d ~/Downloads/
rsync -av ~/Downloads/icons_theme/.local ~
ls -al ~/.local/share/icons
```

### 6.3 Kurzor téma telepítése
```bash
unzip ~/Downloads/cursors-theme.zip -d ~/Downloads/
rsync -av ~/Downloads/cursors_theme/.icons ~
ls -al ~/.icons
```

### 6.4 Betűtípusok és háttérképek telepítése
```bash
unzip ~/Downloads/font-packs.zip -d ~/Downloads/
rsync -av ~/Downloads/fonts/.local ~
ls -al ~/.local/share/fonts
```

## 7. Háttérképek telepítése
```bash
unzip ~/Downloads/wallpaper-gruvbox.zip -d ~/Downloads/
rsync -av ~/Downloads/wallpaper-gruvbox/usr /
ls -al /usr/share/backgrounds/gruvbox
```

## 8. Cinnamon appletek és konfigurációk telepítése
```bash
unzip ~/Downloads/cinnamon-applets-config.zip -d ~/Downloads/
rsync -av ~/Downloads/cinnamon-applets-config/.config ~/
rsync -av ~/Downloads/cinnamon-applets-config/.local ~/
rm -rfv ~/Downloads/cinnamon-applets-config
```

## 9. Téma, ikon, kurzorok, betűtípusok alkalmazása és Cinnamon konfiguráció visszaállítása
```bash
unzip ~/Downloads/cinnamon-config-cinnamenu.zip -d ~/Downloads/
dconf load / > ~/Downloads/cinnamon_config_cinnamenu/cinnamon-config-cinnamenu.conf
```

## 10. Szoftverek:
```
Böngésző > Firefox
Kódszerkesztő > Visual Studio Code, Netbeans
API teszter > Postman
Markdown-néző/-szerkesztő > Haroopad
Konzol > ZSH > Oh-My-Zsh ("bira" téma)
Verziókezelő > Git (GitHub Desktop)
Egyéb > Discord
```
