 <img src="https://flagcdn.com/16x12/us.png" alt="US">  [English (US)](README.md) | <img src="https://flagcdn.com/16x12/br.png" alt="BR">   [Português (BR)](README.pt-br.md)
---
***🛡️ Arch Update Full (Sentinel Protocol)🔄*** **Version 4.1-2**
---

**An advanced, lightweight, and fully automated maintenance tool built for Arch Linux. It centralizes your updates, performance tweaks, and system integrity checks.**

**Arch-Update-Full: The Elite Update Management Protocol for Arch Linux.
Smart synchronization across Pacman, AUR, Flatpaks, and Snaps, paired with real-time integrity auditing. Absolute automation that packs everything you need for updates and routine maintenance (orphan packages and cache purging), while keeping the ultimate control firmly in your hands.**

---
**🚀 What's New: Arch Update Full v: 4.1**

Highlights of the new automation protocol version:

bugs fixe!

**💡 Post-Update Note**
After updating the package via AUR/pacman, run the main script once in your terminal to complete the automatic Sentinel migration or open app desktop.

**​⚜️ Sentinel Module (Smart Notifications):**

Introduction of the dynamic visual alert system with exclusive beacon icons across three levels:
**(The notification button waits 37 minutes before closing as "ignored by the operator"!)**

**🔷 Blue Beacon: Routine updates (low volume).**

**🔶 Yellow Beacon: Moderate volume of pending packages.**

**🔴 Red Beacon Refactored Red Lighthouse: The Red Lighthouse icon is now triggered strictly by package accumulation (= + 34 pending packages), establishing a much clearer alert hierarchy**

**🐧 New Special Icon & Refined Lighthouse Logic:** New Tux with Tools Icon: Added a dedicated notification featuring Tux holding a gear and wrench, exclusively reserved for Kernel and GPU Driver updates.

**⚡ Official Pikaur Support:**
Alongside yay and paru, the script now features complete native integration for the pikaur helper, expanding compatibility for AUR users.

**🧱 Modular Architecture & Isolated Sentinel:**
* Module Decoupling: The Sentinel mode has been separated from the main script into its own dedicated binary (arch-update-full-sentinela), drastically reducing the footprint of the interactive script.

* Race Condition Elimination: Completely eliminates execution conflicts between the user interface and background automated checks.

* Optimized Ghost Operation: The Sentinel runs every 3 hours via systemd --user in total background mode without requiring sudo, triggering notifications only when pending updates exist.

* Self-Healing Mechanism: The main script automatically detects legacy systemd configurations and silently updates the service and timer files to the new path upon its first post-update run.

**📰 Integrated Arch Linux News:**
Now you can read the latest official Arch Linux news directly through the terminal inside arch-update-full, ensuring you know about manual interventions before updating.

**🌐 Interactive Mirrorlist Reflector:**
Mirrorlist optimization via reflector has been improved: now the system explicitly asks if you want to optimize mirrors in the session, giving total network control to the user.

**🎨 Polished Terminal UI/UX & Preparation for Automatic Language Detection:**
Clean, modern, and minimalist CLI interface, using a Neon tone palette for maximum legibility.
**The codebase has been structured to support automatic system language detection in future updates, displaying the terminal directly in PT-BR or EN-US.**

**🌐 Temporary Bilingual Support: Ongoing Multi-Language Support: Initial code restructuring to automatically detect the host system language. Roadmap Languages: Groundwork laid to automatically handle PT-BR (Portuguese), EN-US (English), and ES-ES (Spanish)..**

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
**🛡️ Arch Update Full: Sentinel Protocol (V:4.1)**

arch-update-full has evolved from a simple script into an autonomous maintenance ecosystem. It now executes a rigorous sequence of 16 intelligence and integrity layers, ensuring your Arch Linux remains at the absolute cutting edge of performance and security:

### 🚀 Integrity & Intelligence Layers 

1. **Sentinel Mode (Silent Interception)**: Background monitoring powered by Systemd User Timers. The system silently checks for updates **every 3 hours** and dispatches native alerts via libnotify only when new packages are available.

2. **Dynamic Auto-Installation:** The script features self-configuring logic. Upon execution, it validates its own persistence within the system, ensuring the Sentinel service remains permanently active, regardless of the installation directory.

3. **Mirror Optimization (Reflector):** Dynamically optimizes the *mirrorlist* targeting the 5 fastest, most up-to-date HTTPS servers to maximize your download bandwidth.

4. **Integrity & Core Sync (Pacman):** Performs a deep synchronization of the official repositories and updates critical system core packages.

5. **AUR Intelligence Hub:** Automated discovery of *AUR Helpers*. Features native, intelligent support for **Yay**, **PikAur** or **Paru**, allowing you to choose your update engine on the fly.

6. **Universal Sandbox Update:** Full synchronization of isolated sandbox applications via **Flatpak** and universal packages via **Snapd**, ensuring no sector of the system falls behind.

7. **Disk Integrity Reserve:** Pre-update disk space auditing. If your SSD drops below 5GB of free space, the script executes an emergency purge or aborts the process entirely to prevent data corruption.

8. **Core Audit (Kernel & Driver Check):** Real-time scanning of Pacman logs to flag critical changes to **Nvidia**, **AMD** drivers, the **Linux Kernel**, **Mesa**, or **Systemd**.

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
<img width="533" height="178" alt="imagem aviso de kernel" src="https://github.com/user-attachments/assets/d369f36f-07f2-4141-93bd-32cb3176c5eb" />

<img width="543" height="167" alt="notificação final" src="https://github.com/user-attachments/assets/1b713c33-53a5-4a48-8021-08fff8226f4c" />

---
**Real-time desktop alerts regarding the availability of new updates and immediate confirmation upon completing the maintenance protocol.**

**Icon usage logic:**

<img width="1200" height="896" alt="novo funcionamento arch " src="https://github.com/user-attachments/assets/13c33f4a-e982-4d57-807a-fe0b48a6b256" />

---
## **UI & Visuals**
**CLI: Neon Blue aesthetics featuring detailed logs and a custom signature.**

**Menu: Native desktop integration through a custom application shortcut.**

### **⚡ Sentinel Protocol in Action :**
---

<img width="1043" height="747" alt="1 Imagem colada" src="https://github.com/user-attachments/assets/2afd7c6f-ad3a-45a7-8108-1bf09e0a62e1" />
<img width="1043" height="747" alt="2" src="https://github.com/user-attachments/assets/22ac9771-ad8d-4ec4-a234-f881acf88cd0" />
<img width="1043" height="747" alt="3" src="https://github.com/user-attachments/assets/ad09be6f-ac75-4878-8d65-6dbe56ad9e38" />
<img width="1043" height="747" alt="4" src="https://github.com/user-attachments/assets/4112b789-5f43-4aa7-a6d8-70888b207215" />
<img width="1043" height="747" alt="5" src="https://github.com/user-attachments/assets/838a363f-821e-4c3a-a10b-f715c9ee2ec6" />
<img width="1069" height="763" alt="6" src="https://github.com/user-attachments/assets/d5c2b3e3-d1b9-440c-be0d-504d6598e4d9" />
<img width="1069" height="763" alt="7" src="https://github.com/user-attachments/assets/f6632b02-e6a0-4ed3-b1e3-1214923c6988" />
<img width="1090" height="829" alt="8" src="https://github.com/user-attachments/assets/4909b37f-37ba-41fa-b725-e21c0529fd60" />

https://github.com/user-attachments/assets/8bcd3684-fc2b-434e-99e4-f68bb230f08a

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
---

### 

Created By: **𝕿𝖍𝖊 S𝖊𝖛𝖊𝖓𝖙𝖍** — 𝓦𝓱𝓮𝓻𝓮 𝓲𝓷𝓽𝓮𝓰𝓻𝓲𝓽𝔂 𝓶𝓮𝓮𝓽𝓼 𝓹𝓮𝓻𝓯𝓸𝓻𝓶𝓪𝓷𝓬𝓮. "**

---

🛡️ Developer Profile (Red Team Focus)

**Project Focus:** Shell Automation for Arch Linux Maintenance and Auditing.

**Author:** Gustavo Gianeli (The Seventh)

**Education:** Computer Science Student (Linux enthusiast & tinkerer)


**⚠️ ​Language & Transparency Log: This documentation was originally created by me in Portuguese. Since I am a Computer Science student and currently an English beginner, about 80% of this README was translated and verified with AI assistance, then fully reviewed and adjusted by myself. Using technology every day to reach a global audience !⚠️**
