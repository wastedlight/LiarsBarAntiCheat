# Liar's Bar Anti-Cheat
Credits to [tyzeron](https://github.com/tyzeron/LiarsAntiCheat) for the original BepInEx version which this is based on.

Welcome to the **Liar's Bar Anti-Cheat**!
[Liar's Bar](https://store.steampowered.com/app/3097560/Liars_Bar/)

As a newly launched game, Liar's Bar is still in the process of refining its security features. The development team is actively working to improve these systems and deliver a smoother, more secure gaming experience.

However, due to the game's current P2P setup, cheating remains a significant concern. This mod aims to tackle these challenges by implementing strong anti-cheat protections to safeguard gameplay integrity.

### Current Features
- **Card Obfuscation for Players:**
Protect players from seeing each other's cards by turning all cards into 5 jokers, ensuring a fair experience for everyone.

- **Obfuscation of Played Cards:**
Prevent cheaters from viewing the cards played on the table by transforming them into joker cards, making it impossible to track the game state.

- **Bullet Position Obfuscation:**
Hide the players bullet position from cheaters by displaying the last chamber until death is imminent, at which point the real bullet position is revealed.

- **Automatic Cheater Kicking:**
  - Kick players trying to play cards not in their hand.
  - Kick players attempting to change their bullet position during the game.
  - Kick players who try to place their bullet in an invalid revolver chamber.
  - Kick players attempting to set their own cards via illegal commands.

### Work-In-Progress Features
- **Bullet Rigging Prevention:**
Prevent cheaters from rigging their bullet at the start of the game (currently, the bullet position is dictated on the client side and relayed to the server).

### Planned Features
- **Movement Mod Prevention:**
Prevent modders from using harmless but disruptive mods such as illegal head movements or player body movement.

# Installation
1. Install **MelonLoader** using the [automated installer](https://melonwiki.xyz/#/?id=automated-installation)
2. Launch **Liar's Bar** once with **MelonLoader** installed to generate necessary mod folders and files
3. Navigate to your **Liar's Bar** game directory and go to `./Mods`
    - **Example:** `C:\Program Files (x86)\Steam\steamapps\common\Liar's Bar\Mods`
4. Copy the downloaded **DLL file** (ex. `LiarsAntiCheat.dll`) to the `Mods` folder
5. Launch **Liar's Bar** and enjoy your new Anti-Cheat :)

# Host-Only
Please note that this anti-cheat functions exclusively when you are the host of the lobby. If you join another player's game, the anti-cheat features will not be active, as they rely on server authority.

That said, you can still join other players' lobbies without issue, and it will not affect your ability to play the game.

# Dev Notes
This is a port of tyzeron's original BepInEx anti-cheat to MelonLoader, updated to work with the current version of Liar's Bar. Additional anti-cheat features and fixes have been added on top of the original.

I welcome any feedback you may have on improving or optimizing the code.

---
© Copyright 2024 WastedLight
