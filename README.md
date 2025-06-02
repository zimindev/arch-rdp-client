# 🖥️ RDP Clients for Arch Linux  

A curated list of Remote Desktop Protocol (RDP) clients available for Arch Linux, organized by type.  

---

## 🖥️ **Graphical RDP Clients**  

| Program          | Description                                  | Install Command                  |  
|------------------|----------------------------------------------|-----------------------------------|  
| **Remmina**      | Full-featured GUI client (supports RDP, VNC, SSH) | `sudo pacman -S remmina freerdp` |  
| **KRDC**         | KDE’s built-in remote desktop client        | `sudo pacman -S krdc`             |  
| **GNOME Connections** | Simple RDP/VNC client for GNOME       | `sudo pacman -S gnome-connections` |  
| **Vinagre** *(Legacy)* | Older GNOME remote desktop viewer   | `sudo pacman -S vinagre`          |  

---

## ⌨️ **Terminal-Based / Lightweight Clients**  

| Program          | Description                                  | Install Command                  |  
|------------------|----------------------------------------------|-----------------------------------|  
| **FreeRDP** (`xfreerdp`) | Powerful CLI RDP client (used by Remmina) | `sudo pacman -S freerdp`          |  
| **rdesktop** *(Legacy)* | Older RDP client (less maintained)    | `sudo pacman -S rdesktop`         |  

---

### **Which One Should You Use?**  
- **Best GUI**: **Remmina** (most features, tabs, multi-protocol).  
- **KDE Users**: **KRDC** (integrates with Plasma).  
- **GNOME Users**: **GNOME Connections** (simple and clean).  
- **CLI/Advanced**: **FreeRDP (`xfreerdp`)** (lightweight, scriptable).  

---

### **Example FreeRDP Command**  
```bash
xfreerdp /v:server-ip /u:username /p:password +clipboard /dynamic-resolution
```
*(Flags: `+clipboard` for shared clipboard, `/dynamic-resolution` for resizing)*  
