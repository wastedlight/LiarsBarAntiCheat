# Liar's Bar Anti-Cheat

# Credits to tyzeron for obfuscation stuff (https://github.com/tyzeron/LiarsAntiCheat/releases/tag/v1.0.1)

Welcome to the **Liar's Bar Anti-Cheat**!

[Liar's Bar](https://store.steampowered.com/app/3097560/Liars_Bar/) 

As a newly launched game, Liar's Bar is still in the process of refining its security features. The development team is actively working to improve these systems and deliver a smoother, more secure gaming experience.

However, due to the game's current P2P setup, cheating remains a significant concern. This mod aims to tackle these challenges by implementing strong anti-cheat protections to safeguard gameplay integrity.

### Current Features

- **Card Obfuscation for Players:** 
Protect players from seeing each other’s cards by turning all cards into 5 jokers, ensuring a fair experience for everyone.

- **Obfuscation of Played Cards** 
Prevent cheaters from viewing the cards played on the table by transforming them into joker cards, making it impossible to track the game state..

- **Bullet Position Obfuscation:** 
Hide the players bullet position from cheaters by displaying the last chamber until death is imminent, at which point the real bullet position is revealed.

- **Automatic Cheater Kicking:** 
  - Kick players trying to play cards not in their hand.
  - Kick players attempting to change their bullet position during the game.
  - Kick players who try to place their bullet in an invalid revolver chamber.

### Work-In-Progress Features

- **Bullet Rigging Prevention:** 
Prevent cheaters from rigging their bullet at the start of the game (currently, 
the bullet position is dictated on the client side and relayed to the server).

### Planned Features

- **Movement Mod Prevention:** 
Prevent modders from using harmless but disruptive mods such as illegal head 
movements or player body movement.


# Installation

1. Install **BepInEx** (see [BepInEx Installation Guide](https://docs.bepinex.dev/articles/user_guide/installation/index.html))

2. Launch **Liar's Bar** once with **BepInEx** installed to generate necessary mod folders and files

3. Navigate to your **Liar's Bar** game directory and go to `./BepInEx/plugins`
    - The `BepInEx` and `plugins` folder should have been generated in the previous step
    - **Example:** `C:\Program Files\Steam\steamapps\common\Liar's Bar\BepInEx\plugins`


5. Copy the downloaded **DLL file** (ex. `LiarsBarAntiCheat.dll`) to the `plugins` folder

6. Launch the **Liar's Bar** game and enjoy your new Anti-Cheat :)


# Host-Only

Please note that this anti-cheat functions exclusively when you are the host of the lobby. If you join another player's game, the anti-cheat features will not be active, as they rely on server authority.

That said, you can still join other players' lobbies without issue, and it will not affect your ability to play the game.

# Dev Notes

This anti-cheat  was created within a few hours, so the code may not be as polished due to the rapid pace of development. the primary focus was on functionality over optimization in the initial stages.

I welcome any feedback you may have on improving or optimizing the code.

---

© Copyright 2024 WastedLight
