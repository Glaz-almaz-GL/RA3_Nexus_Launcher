# RA3_Nexus_Launcher

**RA3 Nexus Launcher** is a modern, feature-rich launcher for the game Command & Conquer: Red Alert 3 and its modifications, developed using C# 14, .NET 10, and the Avalonia UI Framework. The interface is inspired by launchers like Corona Launcher and Armor Rush Launcher, using a font based on Red Alert 3 Extended.

**Core Features:**

*   **Game Launching:** Convenient launching of Red Alert 3 with the ability to select installed mods and the game version (defaulting to 1.12).
*   **RA3 QuickLauncher:** Integration with an improved RA3.exe executable for faster game startup times.
*   **Mod Management:** Display a list of installed mods with version information.
*   **Game Settings:**
    *   **Global Params:** Configure screen resolution (including custom), window mode (windowed/fullscreen).
    *   **Player Profiles:** Manage settings for different profiles (LAN/GameSpy IP addresses, `skirmish.ini` repair, enable maps in registry).
    *   **Audio:** Individual volume controls (Ambient, Movie, Music, SFX, Voice) per profile.
    *   **Language:** Select and apply language files (`.csf`) to the game via the registry.
    *   **Launch Parameters:** Ability to specify additional command-line arguments.
*   **Patches & Fixes:** Integrated tools for installing the 4GB Patch, fixing the registry, and generating a new CD key.
*   **RA3BattleNet Support:** Ability to configure and launch the RA3BattleNet client (if installed).
*   **Updates:** Automatic check for updates for the launcher itself.
*   **Interface:** Modern UI using Avalonia.
*   **Notifications:** A notification system for displaying information, warnings, and errors.
*   **Requires Administrator privileges** for specific operations (patching, registry changes).
*   **Detailed Tooltips:** Comprehensive tooltips appear for every UI element, including text labels, buttons, input fields, and dropdown menus, providing detailed descriptions of their functionality and purpose when hovered over. For IP address fields, hovering will display information about the IP type (e.g., Radmin VPN, Hamachi, local network) and its intended usage context.

**Technologies:**

*   **Programming Language:** C# 14
*   **Framework:** .NET 10
*   **UI Toolkit:** Avalonia
*   **Architecture:** MVVM (CommunityToolkit.Mvvm)

**Future Capabilities:**

*   **Localization:** Support for Russian, Chinese, and Arabic languages.
*   **Map Viewer:** An integrated viewer for installed maps, showing the map name, folder name, and a `map.tga` preview, with the option to open the map's location in the file explorer.
*   **Discord Rich Presence (RPC):** Display status on Discord: that the game is running via Nexus Launcher, which mod (or vanilla game) is being played, and whether RA3BattleNet is active.
