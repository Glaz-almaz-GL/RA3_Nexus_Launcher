# RA3 Nexus Launcher

**RA3 Nexus Launcher** is a modern, feature-rich launcher for *Command & Conquer: Red Alert 3* and its modifications, built with **C# 14**, **.NET 10**, and the **Avalonia UI Framework**. The interface draws inspiration from launchers like *Corona Launcher* and *Armor Rush Launcher*, using a custom font based on *Red Alert 3 Extended*.

> ⚠️ **Administrator privileges are required** for operations involving patches and Windows Registry modifications.  
> 💬 **Join our community**: [![Discord](https://img.shields.io/discord/1439871021850165332?color=7289da&label=Discord&logo=discord)](https://discord.gg/tzW856ewKm)

---

## 🔧 Core Features

- **Game Launching**: Select game version (defaults to **1.12**) and installed mod.
- **RA3 QuickLauncher**: Integration with an optimized `RA3.exe` for faster startup.
- **Mod Management**: View a list of installed mods with version information.
- **Game Settings**:
  - **Global Params**: Screen resolution (including custom values), window mode (windowed/fullscreen).
  - **Player Profiles**: Manage LAN/GameSpy IP addresses, auto-repair `skirmish.ini`, register maps in the registry.
  - **Audio**: Independent volume controls (Ambient, Movie, Music, SFX, Voice) per profile.
  - **Language**: Apply `.csf` language files via the Windows Registry.
  - **Launch Parameters**: Specify custom command-line arguments.
- **Tools & Fixes**:
  - Install the **4GB Patch**.
  - Repair registry entries.
  - Generate a new CD key.
- **RA3BattleNet Support**: Configure and launch the RA3BattleNet client (if installed).
- **Auto-updates**: Check for new launcher versions automatically.
- **UI**: Modern Avalonia-based interface following the MVVM pattern (`CommunityToolkit.Mvvm`).
- **Notifications**: Built-in system for info, warning, and error messages.
- **Tooltips**: Comprehensive hover descriptions for every UI element, including IP address types (e.g., Radmin VPN, Hamachi, local network).

---

## 🗺️ Maps Manager (v2.0.0+)

- Browse all installed maps with meta name, description, player count, dimensions, file size.
- Preview map images (`map.tga`) directly in the UI.
- Search by name and filter by exact player count (2, 3, 4…).
- Open the map’s folder in File Explorer with one click.
- View detailed technical information in a dedicated window.

> 💡 Map type (Skirmish/Campaign) is intentionally hidden in the UI to reduce clutter when managing large map collections.

> 🔄 **Map Cache**: Parsed map data is stored in `<Nexus Install Path>/Cache/`. This cache is automatically cleared when you press the **Reload** button in the Maps Manager.

---

## 🎮 Discord Rich Presence

Shows your current activity in Discord:
- That you're using **RA3 Nexus Launcher**.
- The active **game version** and **mod**.
- Whether you're using **RA3BattleNet** or **RadminVPN** for online play.
- An "idle" status when you're in the launcher itself.

---

## 📝 Logging

All launcher actions are logged to timestamped files:  
`<Nexus Install Path>/Logs/Launcher_Log_yyyyMMdd_hhMMss.txt`

Log format example:
```
[2026-01-31 14:33:08.72] [Information] [MODS] Parsed mod info — Name: WOD, Version: 0.091
[2026-01-31 14:33:11.171] [Success] [DISCORD] Discord connection established: glaz_almaz_gl#1049990
...
```

Each entry includes a timestamp, log level, source context (`[MODS]`, `[INI]`, `[PROFILE]`, `[DISCORD]`, etc.), and operation details—enabling efficient troubleshooting and auditability.

---

## ⚙️ Technology Stack

| Component        | Implementation                     |
|------------------|------------------------------------|
| Language         | C# 14                              |
| Runtime          | .NET 10                            |
| UI Framework     | Avalonia                           |
| Architecture     | MVVM (`CommunityToolkit.Mvvm`)     |
| Async Handling   | `CancellationTokenSource`, `Task.Run` |
| Configuration    | JSON (`%AppData%\RA3 Nexus Launcher\settings.json`) |

---

## 🌍 Future Plans

- **Localization**: Russian, Chinese, and Arabic support.
- **NuGet Package**: A developer-friendly library for RA3 integration (handling `.ini`, `.csf`, `map.tga`, registry keys, CD-key generation, etc.).
- **Advanced Map Viewer**: Texture previews, property inspection, metadata export.
- **Multi-language UI**: Launcher interface available in multiple languages.
- **Enhanced Mod Update System**: GitHub-based mod version tracking and notifications.

---

## 📸 Screenshots

### Main Menu  
![Main Menu](https://github.com/user-attachments/assets/ef5ea3a6-20d8-499d-af55-626b4d4df57a)

### Settings — General & Audio  
![Settings General](https://github.com/user-attachments/assets/d19bc3a5-dffb-4033-8ffd-51a9492e7886)  
![Settings Audio](https://github.com/user-attachments/assets/3b7b04f3-18e2-46ff-8d66-c7c0e2df3d64)  
![Settings Language & Launch](https://github.com/user-attachments/assets/cc7eea83-9cf0-4e1a-8446-2ca2d0b4907f)

### Maps Manager  
![Maps Manager Overview](https://github.com/user-attachments/assets/60813296-fd34-499a-80c1-7b08ef923d5b)  
![Map Details Dialog](https://github.com/user-attachments/assets/e880ce4b-0701-456d-b899-82fccc6f1067)

### Discord Rich Presence  
![Discord Status — In Launcher](https://github.com/user-attachments/assets/f21f41d6-12b2-42e2-92e3-5947242d5310)  
![Discord Status — In-Game](https://github.com/user-attachments/assets/cbb39ef3-2354-4173-b79c-444eda1109f5)

---

## 📥 Installation & Usage

1. Download the latest release from [Releases](https://github.com/your-repo/RA3-Nexus-Launcher/releases).
2. Extract the archive to any directory (this becomes your *Nexus Install Path*).
3. Run `RA3NexusLauncher.exe`.
4. If required, the launcher will automatically restart with administrator privileges.

Configuration is stored at:  
`%AppData%\RA3 Nexus Launcher\settings.json`

---

## 💬 Community & Support

Join our official Discord server to get help, share feedback, or discuss modding:

🔗 [**Join RA3 Nexus Launcher Discord**](https://discord.gg/tzW856ewKm)
---

> 🛠️ **Developer**: Glaz_almaz  
> 📌 **Recommendation**: Install the **4GB Patch** before running large mods to prevent crashes.

---

**Commanders — to battle!** 🚀  
Thank you for using **RA3 Nexus Launcher**.
