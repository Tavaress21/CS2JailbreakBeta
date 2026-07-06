# TavaresJB — Jailbreak Plugin for CS2
###If you find any bugs, or want to add features: discord luistavares

Welcome to the official documentation for the **TavaresJB** plugin, a comprehensive Jailbreak solution for Counter-Strike 2, developed using the CounterStrikeSharp framework[cite: 1].

## 📋 Overview
TavaresJB is organized into modular components to ensure clean maintenance and scalability. Each module communicates through a central `JailbreakPlugin` class[cite: 1].

### Key Features
*   **Warden System**: Complete control over cells, bunny hop, block, game days, and last requests[cite: 1].
*   **Administration**: Full control suite including Kick/Ban, Slap/Slay, NoClip, GodMode, Bury, and Revive[cite: 1].
*   **VIP System**: Exclusive perks per round and a dedicated point-based system[cite: 1].
*   **Economy & Shop**: Integrated credit system earned through playtime and eliminations, used to purchase shop items or VIP status[cite: 1].
*   **Gangs**: Create and join groups with custom tags and names[cite: 1].
*   **Last Request (LR)**: 9 unique 1v1 duel types[cite: 1].
*   **Game Days**: 12 diverse modes including Freeze Tag, Hide and Seek, Spartan, and more[cite: 1].
*   **Persistence**: Uses an SQLite database to save player stats, skins, and VIP status[cite: 1].

## 🎮 Commands Reference

### Chat Commands (`!command`)
| Command | Access | Description |
| :--- | :--- | :--- |
| `!menu` | All | Opens the main Jailbreak menu |
| `!shop` / `!loja` | All | Opens the credit shop |
| `!skin` / `!skins` | All | Opens the character skin menu |
| `!vipmenu` | VIP | Opens the VIP benefits menu |
| `!gang` | All | Gang management menu |
| `!days` | Warden | Opens the Game Days submenu |
| `!adminmenu` | Admin | Opens the full admin panel |

### Console Commands
*   `css_menu`: Opens the main menu (ideal for binds: `bind m "css_menu"`)[cite: 1].
*   `css_warden`: Grants Warden status or reopens the Warden menu[cite: 1].
*   `css_vip`: Opens the VIP menu[cite: 1].
*   `css_jbday <id>`: Starts a Game Day directly[cite: 1].

## 🛡️ Permissions System
The plugin utilizes the native CounterStrikeSharp permission flags (`@css/root`, `@css/generic`, `@css/warden`) to manage access[cite: 1].

> **Note**: The server owner's SteamID64 is hardcoded in `PermissionsManager.cs` for a permanent total-access bypass[cite: 1].

## ⚙️ Configuration
The `config.json` file allows for full customization without needing to recompile the source code, including:
*   `VipCostPerDay`: Cost to purchase VIP status[cite: 1].
*   `RebelOptionsMinGuardsForAnyone`: Threshold for public vs. Admin access to Rebel Options[cite: 1].
*   `CellTriggerNames`: Configurable map-specific cell trigger names[cite: 1].

---

*This plugin is currently in version **0.3.0**. For more details, refer to the full technical documentation in **TavaresJB-documentacao.html**[cite: 1].*
