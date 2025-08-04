# gentoo-dotfiles

Personal dotfiles for my Gentoo system.  
KDE Plasma (Wayland), systemd, chezmoi-managed.

---

## Features

- Managed with [`chezmoi`](https://www.chezmoi.io/)
- KDE Plasma configuration for Wayland
- Clean terminal setup using `kitty`
- Includes:
  - `.bashrc`, `.bash_profile`, `.profile`
  - `.gitconfig`
  - KDE settings (`kdeglobals`, `plasmarc`, `kwinrc`)
  - Systemd user units (e.g. PipeWire)
  - Fonts, cursor themes
  - `emerge-info.txt` and `world.bak` for rebuilds

---

## Setup

### 1. Install chezmoi

```bash
sh -c "$(curl -fsLS get.chezmoi.io)"
```

Or on Gentoo:

```bash
emerge --ask app-admin/chezmoi
```

### 2. Apply dotfiles

```bash
chezmoi init andrgv
chezmoi apply
```

This applies all tracked config files to `~`.

---

## References

- [chezmoi docs](https://www.chezmoi.io/docs/)
- [Gentoo Wiki: Dotfiles](https://wiki.gentoo.org/wiki/Dotfiles)
- [Gentoo Wiki: Systemd](https://wiki.gentoo.org/wiki/Systemd)
- [KDE config reference](https://userbase.kde.org/)
