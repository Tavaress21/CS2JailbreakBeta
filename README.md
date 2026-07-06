# TavaresJB — Jailbreak Plugin for CS2

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

## 🎯 Game Days (12 Modes)
Special modes triggered by the Warden that modify mechanics for the round duration[cite: 1].
*   **Freeze Tag**: Players have multiple lives; being hit freezes you until an ally unthaws you[cite: 1].
*   **Hide and Seek**: Guards are frozen and blinded during the hiding phase[cite: 1].
*   **War Day**: Generic modifier engine for custom weapon/health/gravity setups[cite: 1].
*   **Gravity Day**: Reduced gravity for all players[cite: 1].
*   **Spartan Day**: Guards limited to Glocks; prisoners have 300 HP[cite: 1].
*   **Zombie Day**: Zombies have knives and 900 HP; survivors have AK-47s[cite: 1].
*   **Reverse Zombie Day**: Roles swapped from standard Zombie Day[cite: 1].
*   **DeathMatch Day**: Everyone receives a random weapon for a free-for-all[cite: 1].
*   **Night Crawler Day**: Guards move in total silence while hunting[cite: 1].
*   **Reverse Night Crawler**: Movement advantage swapped[cite: 1].
*   **Gang Day**: Terrorists split into two gangs; friendly fire enabled[cite: 1].
*   **Midnight Nade War**: Terrorists-only; fight using 3 HE grenades[cite: 1].

## ⚔️ Last Request (9 Duels)
Initiated when exactly one Terrorist is alive. The Warden picks the duel type, and the prisoner chooses the guard[cite: 1].
*   **Shot4Shot**: Trading shots with the same weapon[cite: 1].
*   **Knife Fight**: Melee duel[cite: 1].
*   **No Scope**: Sniper scope zooming blocked[cite: 1].
*   **Pistols**: Pistols-only duel[cite: 1].
*   **Gun Toss**: Struggle for weapon control[cite: 1].
*   **Race**: Foot race to a map destination[cite: 1].
*   **Grenade Duel**: Limited grenades for both[cite: 1].
*   **Scout Duel**: Scouts under low gravity[cite: 1].
*   **Suicide Bomber**: Prisoner detonates C4 using the "Use" key[cite: 1].

## 🛡️ Permissions System
The plugin utilizes the native CounterStrikeSharp permission flags (`@css/root`, `@css/generic`, `@css/warden`)[cite: 1].
> **Note**: The server owner's SteamID64 is hardcoded in `PermissionsManager.cs` for a permanent total-access bypass[cite: 1].

## ⚙️ Configuration
The `config.json` file allows for full customization including `VipCostPerDay`, `RebelOptionsMinGuardsForAnyone`, and map-specific `CellTriggerNames`[cite: 1].

---

*This plugin is currently in version **0.3.0**. For more details, refer to the full technical documentation in ***DISCORD: luistavares***
