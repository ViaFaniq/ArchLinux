# ArchLinux  
Helpful Commands and Setup Notes

---

### 🖥️ Hyprland Installation (Arch Minimal)

- **Installation Script:**  
  [https://github.com/JaKooLit/Arch-Hyprland](https://github.com/JaKooLit/Arch-Hyprland)

- **Video Guide:**  
  [YouTube – Hyprland Installation Tutorial](https://www.youtube.com/watch?v=lR7EtbVYWuc&t=540s)

---

### 🎮 Game Optimization on Linux (It doesn't work on Hyprland)

1. Install required packages: 
   ```bash
   sudo pacman -S gamescope gamemode

2. In the game’s launch options, paste:
   ```bash
   gamemoderun gamescope -W 1920 -H 1080 -r 75 --force-grab-cursor -f -- %command%

---

### 🖨️ Printer Drivers (Canon and More)

1. Install CUPS:
   ```bash
   sudo pacman -S cups
2. Install Canon printer and scanner drivers:
   ```bash
   yay -S cnijfilter2 scangearmp2
3. Enable and start the CUPS service:
   ```bash
   sudo systemctl enable cups
   sudo systemctl start cups
4. Open the CUPS configuration in your browser:
   ```bash
   http://localhost:631

---

### 🍙 App Image Launcher

1. Install:
   ```bash
   yay -S appimagelauncher

---


### 🔲 Windows Fix Time DualBoot

1. Open Cmd as admin:
   ```bash
   reg add "HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\TimeZoneInformation" /v RealTimeIsUniversal /d 1 /t REG_DWORD /f

---
