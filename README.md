🌐 **Languages / Idiomas:** <img src="https://flagcdn.com/16x12/us.png" alt="US"> **🇺🇸**  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR"> **🇧🇷**  [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Sentinel Protocol)🔄*** **Version 3.8**
---

**An advanced, lightweight, and fully automated maintenance tool built for Arch Linux. It centralizes your updates, performance tweaks, and system integrity checks.**

**Arch-Update-Full: The ultimate management protocol for Arch Linux updates. Smart sync across Pacman, AUR, Flatpaks, and Snaps with real-time integrity auditing. Full automation that handles everything you need for routine updates and system maintenance (orphan packages and cache cleanup).**

---
**🚀 What's New: Arch Update Full v3.8 (Sentinel Update)**
 **Highlights of the latest release:**

**⚡ Smart Connectivity Gatekeeper:** A pre-verification network system that checks your connection before starting critical processes, preventing timeouts and database corruption.

**📊 Real-time Latency Telemetry:** Accurate latency extraction using AWK, showing network status in milliseconds (ms) directly on the interface.

**🎨 UI Redesign (Block Edition):** Next-Gen UI Architecture featuring double-character borders and dynamic alignment for an immersive, professional terminal experience.

**🧹 Orphan Package Bug Fix:** Fixed the bug related to orphan package removal, ensuring a clean and automated purge.

**🛡️ Conflict Mediation:** Strategic removal of the `--noconfirm` flag from Pacman to allow manual validation during critical package changes, keeping your system fully stable.

**✅ ShellCheck Certified: 100% validated code**. Zero syntax or logic errors, ensuring maximum stability on Bash.

--- 
**📦 Installation (AUR): **Arch Update Full is available on the AUR. This is the recommended installation method because it ensures the package** itself stays updated through the AUR repository. 🔄🛡️**
--- 

**👉  Official AUR Repository: https://aur.archlinux.org/packages/arch-update-full**

**⚠️ AUR Version Note:** In the AUR repository, the package is currently at version 3.8-7. The -7 suffix represents purely packaging revisions (pkgrel) made during deployment (such as checksum fixes and icon path adjustments). The core source code and features remain identical to the stable 3.8 release found in this repository.❗


### 🚀 **Quick Installation (AUR Helpers)**
**Deploy the package automatically using your preferred AUR manager:**

 **➡ Install utilizing Yay:** 
```bash
yay -S arch-update-full
```
 **➡ Install utilizing Paru**
```bash
paru -S arch-update-full
```

---
# **🛠️ Protocol Architecture (Core Functions)**
**🛡️ Arch Update Full: Sentinel Protocol (v3.8)**

arch-update-full evolved from a simple script into an autonomous maintenance ecosystem. It runs a strict sequence of 14 integrity and intelligence layers, making sure your Arch Linux setup stays at peak performance and security:

### 🚀 Integrity and Intelligence Layers (Sentinel Protocol)

1. **Sentinel Mode (Silent Interception):** Background monitoring running via *Systemd User Timers*. The system checks for updates silently **every 3 hours** and sends native desktop alerts via `libnotify` only if new packages are available.

2. **Dynamic Auto-Installation:** Built-in self-configuration logic. When executed, the script checks its own persistence in the system, making sure the Sentinel service stays active no matter which folder it was installed in.

3. **Mirror Optimization (Reflector):** Dynamically optimizes your *mirrorlist* to target the 5 fastest and most synced HTTPS servers, maximizing your download speeds.

4. **Integrity & Core Sync (Pacman):** Deep sync of official repositories and core system updates.

5. **AUR Intelligence Hub:** Auto-detects your *AUR Helpers*. It has native support for **Yay** or **Paru**, letting you choose the update engine on the fly.

6. **Universal Sandbox Update:** Full sync for sandboxed apps via **Flatpak** and universal packages via **Snapd**, ensuring no part of your system gets left behind.

7. **Disk Integrity Reserve:** Pre-update disk space check. If your SSD has less than 5GB free, the script runs an emergency cleanup or aborts the process to prevent data corruption.

8. **Core Auditing (Kernel & Driver Check):** Real-time scans of Pacman logs to spot critical changes in **Nvidia** drivers, the **Linux Kernel**, **Mesa**, or **Systemd**.

9. **Orphan Purge & Cache Cleanup:** Finds and removes leftover dependencies (orphans) and manages your system cache using `paccache`, `paccache -r`, and the `pacman -Sc` command, extending your SSD's lifespan.

10. **Sentinel Logs (FIFO Rotation):** A rolling log system. The script keeps only the last 13 update sessions, giving you enough history for debugging without cluttering your storage.

11. **Universal Notification Protocol:** When the maintenance cycle finishes or finds an update (in ghost/sentinel mode), the script fires a desktop alert via `libnotify`. This ensures that on **any desktop environment (DE) or window manager**, even if you are on another workspace or focused on your studies, you get immediate confirmation that **Sentinel** completed its task, updates were detected, and logs were generated.

12. **📊 Telemetry System (Logs)**
The protocol manages two independent log streams:
* `~/.logs_arch_update_full/` -> Full history of manual sessions (retains 13 versions).
* `~/.logs_sentinel_check/` -> Technical logs of background Sentinel rounds (retains 3 versions).

13. **ShellCheck Validation (Quality Certification):** The code was run through ShellCheck and passed with zero errors. This guarantees flawless Bash syntax, properly quoted variables, and eliminates the risk of silent failures from bad commands. Fully armored code.

14. **⚡ Smart Connectivity Gatekeeper:** A pre-verification network system that checks your connection before starting critical processes, preventing timeouts and database corruption.

--- 
### 🔔 Smart Notifications
---

**Real-time desktop alerts for new update availability and instant confirmation as soon as the maintenance cycle finishes.**

<img width="1752" height="681" alt="sentinela avisando updates" src="https://github.com/user-attachments/assets/9f993c59-dd7a-4fc3-b12b-1b4d640b18f8" />
<img width="1774" height="643" alt="captura protocolo concluido" src="https://github.com/user-attachments/assets/31cbd1a7-9430-4a3a-8654-c721fec45e39" />


---
## **📸 UI & Visuals**
**CLI: Neon Blue aesthetics featuring detailed logs and a custom signature.**

**Menu: Native desktop integration through a custom application shortcut.**

### **⚡ Sentinel Protocol in Action : ⬇**
---
<img width="1433" height="1033" alt="cap1" src="https://github.com/user-attachments/assets/5a95455a-2708-4bfb-8f2b-a31dd3185c52" />
<img width="1433" height="1033" alt="cap2" src="https://github.com/user-attachments/assets/7de9989b-4221-4f56-b3b3-6ee3bab39db4" />
<img width="1433" height="1033" alt="cap3" src="https://github.com/user-attachments/assets/c2b1cf9a-c935-44c7-b1ed-47ae43a4a332" />
<img width="1433" height="1033" alt="cap4" src="https://github.com/user-attachments/assets/70bf79bb-1fb5-4fd7-968a-d80597f130ca" />
<img width="1433" height="1033" alt="cap5" src="https://github.com/user-attachments/assets/19a2f731-8222-4460-92bc-8a1be5482e4c" />


### **🚀 System Menu (v3.8 Feature!)**
---
<img width="256" height="256" alt="sentinela-v38" src="https://github.com/user-attachments/assets/fc7c7948-820a-434d-9c03-0e373a2b1e69" />

### **📁 Log File Location: /home/$USER/.** (~/.logs_arch_update_full/  &  ~/.logs_sentinel_check/)
---
<img width="325" height="180" alt="pasta de logs" src="https://github.com/user-attachments/assets/ca450a3c-da95-4c5f-a6ba-e4d972e9030e" />
<img width="2012" height="1288" alt="logs script completo" src="https://github.com/user-attachments/assets/e06d5d27-fa6b-4eb0-9aca-21aee2b79419" />
<img width="2012" height="1288" alt="logs do sentinela" src="https://github.com/user-attachments/assets/dc240133-891a-4e14-acfe-2499b38520e0" />


---
### 🚀 **⚠️ WE HIGHLY RECOMMEND INSTALLING VIA THE AUR PACKAGE⚠️**

***...but if you prefer doing it manually...***

**How to Install Manually:**
---

**➡ To use the script as a native command and get the shortcut in your applications menu, run the following commands:**
```bash
git clone https://aur.archlinux.org/arch-update-full.git
cd arch-update-full
makepkg -si
```
**➡ Or, if you prefer to deploy the files directly and manually:**

**1. Inject the script into your system PATH:**
```bash
sudo cp arch-update-full /usr/bin/arch-update-full
sudo chmod 755 /usr/bin/arch-update-full
```
**2. Move the icon to the system pixmaps directory:**
```bash
sudo cp sentinela-v38.png /usr/share/pixmaps/
```
**3. Install the shortcut into the applications menu (XDG):**
```bash
sudo cp arch-update-full.desktop /usr/share/applications/
```
---

**🚀 Arch Update Full - - - Sentinel Protocol**

---
### **𝓓𝓮𝓿𝓮𝓵𝓸𝓹𝓮𝓭 𝓫𝔂 𝓖𝓾𝓼𝓽𝓪𝓿𝓸 𝓖𝓲𝓪𝓷𝓮𝓵𝓲  (𝓣𝓱𝓮 𝓢𝓮𝓿𝓮𝓷𝓽𝓱)**  

**" 𝓓𝓮𝓿𝓮𝓵𝓸𝓹𝓮𝓭 𝓫𝔂 𝓣𝓱𝓮 𝓢𝓮𝓿𝓮𝓷𝓽𝓱 — 𝓦𝓱𝓮𝓻𝓮 𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓽𝔂 𝓶𝓮𝓮𝓽𝓼 𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮. 🍀 "**

---

🛡️ Developer Profile (Red Team Focus)

**Project Focus:** Shell Automation for Arch Linux Maintenance and Auditing.

**Author:** Gustavo Gianeli (The Seventh)

**Education:** Computer Science Student (Linux enthusiast & tinkerer)

**Hardware:** Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

**Location:** Ourinhos, SP - Brazil

### ***⚠️ ​🌐❗Language & Transparency Log: This documentation was originally created by me in Portuguese. Since I am a Computer Science student and currently an English beginner, about 80% of this README was translated and verified with AI assistance, then fully reviewed and adjusted by myself. Please excuse any minor translation bugs. Using technology every day to reach a global audience ! 🚀❗🙏🍃***
