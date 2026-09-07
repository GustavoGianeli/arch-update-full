 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">   [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Sentinel Protocol)🔄*** **Version 4.0**
---

**An advanced, lightweight, and fully automated maintenance tool built for Arch Linux. It centralizes your updates, performance tweaks, and system integrity checks.**

**Arch-Update-Full: The Elite Update Management Protocol for Arch Linux.
Smart synchronization across Pacman, AUR, Flatpaks, and Snaps, paired with real-time integrity auditing. Absolute automation that packs everything you need for updates and routine maintenance (orphan packages and cache purging), while keeping the ultimate control firmly in your hands.**

---
**🚀 What's New: Arch Update Full v: 4.0**
Highlights of the new automation protocol version:

**Sentinel Module (Smart Notifications):**
Introduction of the dynamic visual alert system with exclusive beacon icons across three levels:

**🔷 Blue Beacon: Routine updates (low volume).**

**🔶 Yellow Beacon: Moderate volume of pending packages.**

**🔴 Red Beacon / Kernel Tux: Critical alert (Kernel, NVIDIA/Mesa drivers, Systemd) requiring attention and suggesting a system reboot.**

**⚡ Official Pikaur Support:**
Alongside yay and paru, the script now features complete native integration for the pikaur helper, expanding compatibility for AUR users.

**🧱 Modular Architecture (Refactored Code):**
The code is no longer an extensive monolithic script and has been completely rebuilt into independent, readable functions orchestrated by a clean and performant main() function.

**📰 Integrated Arch Linux News:**
Now you can read the latest official Arch Linux news directly through the terminal inside arch-update-full, ensuring you know about manual interventions before updating.

**🌐 Interactive Mirrorlist Reflector:**
Mirrorlist optimization via reflector has been improved: now the system explicitly asks if you want to optimize mirrors in the session, giving total network control to the user.

**🎨 Polished Terminal UI/UX & Preparation for Automatic Language Detection:**
Clean, modern, and minimalist CLI interface, using a Neon tone palette for maximum legibility.
**The codebase has been structured to support automatic system language detection in future updates, displaying the terminal directly in PT-BR or EN-US.**

**🌐 Temporary Bilingual Support: To embrace our global community, terminal outputs now feature dual side-by-side text (PT-BR and EN-US).**

✅ **ShellCheck Certified: 100% validated code**. Zero syntax and logic errors, ensuring maximum stability in Bash.

---
**📦 Installation (AUR): Arch Update Full is available on the AUR. This is the recommended installation method to keep the software always updated.**
---

**👉 Package link on AUR: https://aur.archlinux.org/packages/arch-update-full**

### 🚀 **Quick Installation (AUR Helpers)**
**Choose your preferred AUR helper to automatically sync and install the package:**

 **➡ Install utilizing Yay:** 
```bash
yay -S arch-update-full
```
 **➡ Install utilizing Paru**
```bash
paru -S arch-update-full
```
 **➡ Install utilizing Pikaur:**
```bash
pikaur -S arch-update-full
```

---
# **Protocol Architecture (Core Functions)**
**🛡️ Arch Update Full: Sentinel Protocol (V:4.0)**

arch-update-full has evolved from a simple script into an autonomous maintenance ecosystem. It now executes a rigorous sequence of 16 intelligence and integrity layers, ensuring your Arch Linux remains at the absolute cutting edge of performance and security:

### 🚀 Integrity & Intelligence Layers 

1. **Sentinel Mode (Silent Interception)**: Background monitoring powered by Systemd User Timers. The system silently checks for updates **every 3 hours** and dispatches native alerts via libnotify only when new packages are available.

2. **Dynamic Auto-Installation:** The script features self-configuring logic. Upon execution, it validates its own persistence within the system, ensuring the Sentinel service remains permanently active, regardless of the installation directory.

3. **Mirror Optimization (Reflector):** Dynamically optimizes the *mirrorlist* targeting the 5 fastest, most up-to-date HTTPS servers to maximize your download bandwidth.

4. **Integrity & Core Sync (Pacman):** Performs a deep synchronization of the official repositories and updates critical system core packages.

5. **AUR Intelligence Hub:** Automated discovery of *AUR Helpers*. Features native, intelligent support for **Yay** or **Paru**, allowing you to choose your update engine on the fly.

6. **Universal Sandbox Update:** Full synchronization of isolated sandbox applications via **Flatpak** and universal packages via **Snapd**, ensuring no sector of the system falls behind.

7. **Disk Integrity Reserve:** Pre-update disk space auditing. If your SSD drops below 5GB of free space, the script executes an emergency purge or aborts the process entirely to prevent data corruption.

8. **Core Audit (Kernel & Driver Check):** Real-time scanning of Pacman logs to flag critical changes to **Nvidia** drivers, the **Linux Kernel**, **Mesa**, or **Systemd**.

9. **Orphan & Cache Purge:** Locates and sweeps away residual dependencies (orphans) while stabilizing the package cache—retaining the last 3 versions via `paccache`, `paccache -r`, and `pacman -Sc`—to preserve your SSD’s lifespan.

10. **Sentinel Logs (FIFO Rotation):** A telemetry setup utilizing rotating logs. The script retains only the last 13 update sessions, ensuring a reliable debugging history without hoarding storage space.

11. **Universal Notification Protocol:** Upon completing the maintenance loop or detecting an update (Sentinel Ghost Mode), the script dispatches a desktop alert via `libnotify`. This guarantees that across **any interface or Desktop Environment (DE)**—even if you are on another workspace or locked in on your studies—you get instant confirmation that the **Sentinel** has finished its run, detected updates, and successfully written the logs.

12. **Interactive Notifications ((Sentinel Mode NOW with custom notification icons)): The background daemon now fires up a smart visual alert featuring a "Click to Launch App" button. Clicking it instantly triggers the native .desktop launcher, spawning the terminal right in front of you.** 
    
13. **Telemetry System (Logs)**
The protocol manages two independent log streams:
**~/.logs_arch_update_full/:** Complete history of manual sessions (13-version retention).
**~/.logs_sentinel_check/:** Technical logs tracking the Sentinel’s routine rounds (3-version retention).

14. **ShellCheck Validation (Quality Certification)** The Standard: The entire codebase went through the ShellCheck gauntlet and emerged with zero errors. Result: This ensures the Bash syntax is pristine, variables are safely quoted, and there is absolutely zero risk of silent failures due to malformed commands. It's a completely bulletproof codebase.

15. **Smart Connectivity Gatekeeper:** Network testing has been significantly upgraded. The protocol now runs a primary ping against your local mirrors. If there is no response, a secondary fallback attempt is made directly to archlinux.org before aborting the operation.

16. **Hybrid AUR Updates: Absolute control is back in your hands. You can now choose your preferred operational mode on the fly when updating the AUR:**
**Automatic: Executes a rapid, hands-off update (--noconfirm).**
**Manual: An interactive mode where you can audit PKGBUILDs and confirm changes step-by-step ([!] defaults to manual mode as a safety fallback in case of user typos).**

---

**Smart Notifications**

---

<img width="620" height="241" alt="notificação sentila azul" src="https://github.com/user-attachments/assets/e1379b74-e5da-4fd9-895c-29f9940d6c18" />
<img width="678" height="261" alt="notificação vermelha" src="https://github.com/user-attachments/assets/fb869b96-7911-4d40-88e5-7be5d289bc74" />
<img width="543" height="167" alt="notificação final" src="https://github.com/user-attachments/assets/1b713c33-53a5-4a48-8021-08fff8226f4c" />

**Real-time desktop alerts regarding the availability of new updates and immediate confirmation upon completing the maintenance protocol.**

**Icon usage logic:**
<img width="1254" height="1254" alt="logica farol atualizado" src="https://github.com/user-attachments/assets/f8eddfb3-94dd-49ef-ad30-e8d96516de29" />

---
## **UI & Visuals**
**CLI: Neon Blue aesthetics featuring detailed logs and a custom signature.**

**Menu: Native desktop integration through a custom application shortcut.**

### **⚡ Sentinel Protocol in Action :**
---

<img width="1165" height="863" alt="1" src="https://github.com/user-attachments/assets/fc1ed2d1-bb2d-4e4d-abfb-9182dff574d9" />
<img width="1165" height="863" alt="2" src="https://github.com/user-attachments/assets/366421a2-25f0-4a0a-8acd-1ef8bca4979a" />
<img width="1165" height="863" alt="3" src="https://github.com/user-attachments/assets/647398c4-3371-46a6-863e-cba198a2e966" />
<img width="1165" height="863" alt="4" src="https://github.com/user-attachments/assets/a23f5a2f-f38d-4065-91e2-aa794b318868" />
<img width="1165" height="863" alt="5" src="https://github.com/user-attachments/assets/a82bb590-5b1c-4a9b-a927-11128bba6be7" />
<img width="1165" height="863" alt="6" src="https://github.com/user-attachments/assets/000a1568-a08d-47a8-8f27-491aa1a74d3b" />
<img width="1165" height="863" alt="7" src="https://github.com/user-attachments/assets/62917bd5-9de7-4f9c-93d4-0995d7d48990" />
<img width="1165" height="863" alt="8" src="https://github.com/user-attachments/assets/c6c8cce2-2551-45ac-999a-cb2f882388fa" />
<img width="1165" height="863" alt="9" src="https://github.com/user-attachments/assets/74a4b5dd-f2d1-4806-9692-773a6a8884e3" />

https://github.com/user-attachments/assets/56ae70dc-ea84-4852-b0b8-feb36229ce8f


### **🚀 System Menu**
---
<img width="512" height="512" alt="novalogoarchupdatefullv39" src="https://github.com/user-attachments/assets/ff0b5bf6-a321-43ba-8605-59120d781b0e" />


### **📁 Log File Location: /home/$USER/.** (~/.logs_arch_update_full/  &  ~/.logs_sentinel_check/)
---
<img width="325" height="180" alt="pasta de logs" src="https://github.com/user-attachments/assets/ca450a3c-da95-4c5f-a6ba-e4d972e9030e" />
<img width="2012" height="1288" alt="logs script completo" src="https://github.com/user-attachments/assets/e06d5d27-fa6b-4eb0-9aca-21aee2b79419" />
<img width="2012" height="1288" alt="logs do sentinela" src="https://github.com/user-attachments/assets/dc240133-891a-4e14-acfe-2499b38520e0" />


---
**⚠️ WE HIGHLY RECOMMEND INSTALLING VIA THE AUR PACKAGE⚠️**

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
sudo cp novalogoarchupdatefullv39.png /usr/share/pixmaps/
```
**3. Install the shortcut into the applications menu (XDG):**
```bash
sudo cp arch-update-full.desktop /usr/share/applications/arch-update-full.desktop
```
**4. Install Sentinel Module icons (Notification Beacons):**
```bash
sudo mkdir -p /usr/share/arch-update-full/icons
sudo cp farol_azul_simbolo.png /usr/share/arch-update-full/icons/
sudo cp farol_amarelo_simbolo.png /usr/share/arch-update-full/icons/
sudo cp farol_vermelho_simbolo.png /usr/share/arch-update-full/icons/
```
---

### **𝓓𝓮𝓿𝓮𝓵𝓸𝓹𝓮𝓭 𝓫𝔂 𝓖𝓾𝓼𝓽𝓪𝓿𝓸 𝓖𝓲𝓪𝓷𝓮𝓵𝓲  (𝓣𝓱𝓮_ 𝓢𝓮𝓿𝓮𝓷𝓽𝓱)**  

**" 𝓓𝓮𝓿𝓮𝓵𝓸𝓹𝓮𝓭 𝓫𝔂 𝓣𝓱𝓮_ 𝓢𝓮𝓿𝓮𝓷𝓽𝓱 — 𝓦𝓱𝓮𝓻𝓮 𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓽𝔂 𝓶𝓮𝓮𝓽𝓼 𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮. "**

---

🛡️ Developer Profile (Red Team Focus)

**Project Focus:** Shell Automation for Arch Linux Maintenance and Auditing.

**Author:** Gustavo Gianeli (The Seventh)

**Education:** Computer Science Student (Linux enthusiast & tinkerer)

**Hardware:** Acer Nitro V15 | i7 13th Gen | RTX 4050 | 32GB RAM

**Location:** Ourinhos, SP - Brazil

**⚠️ ​Language & Transparency Log: This documentation was originally created by me in Portuguese. Since I am a Computer Science student and currently an English beginner, about 80% of this README was translated and verified with AI assistance, then fully reviewed and adjusted by myself. Using technology every day to reach a global audience !⚠️**
