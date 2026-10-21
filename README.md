# Roblox FPS Prototype

A lightweight Roblox FPS game prototype built for both PC and mobile play. This project is meant to be a clean starting point for building a fast, beginner-friendly first-person shooter with shared gameplay logic for keyboard + mouse and touch controls.

## Overview

This repository includes:

- PC controls for mouse and keyboard
- Mobile controls for touch input
- Basic shooting system
- Health and damage handling
- Respawn flow
- Simple arena structure
- Clean project organization for future expansion

This is a starter repo for learning how to build a Roblox FPS in a way that works across multiple input types.

## Project Goals

- Create a playable first-person shooter prototype
- Support both PC and mobile players
- Keep logic simple and readable for beginners
- Separate client input from server-side validation
- Serve as a foundation for larger game modes later

## Recommended Structure

```text
RobloxFPSPrototype/
├── README.md
├── docs/
│   ├── controls.md
│   ├── roadmap.md
│   └── gameplay-notes.md
├── scripts/
│   ├── Client/
│   │   ├── Input.lua
│   │   ├── CameraController.lua
│   │   └── GunClient.lua
│   ├── Server/
│   │   ├── CombatServer.lua
│   │   ├── HealthSystem.lua
│   │   └── MatchManager.lua
│   └── Shared/
│       ├── Config.lua
│       └── Utility.lua
├── assets/
│   └── ui/
└── game/
    └── arena/
```

## Controls

### PC

- W/A/S/D: Move
- Mouse: Aim
- Left Click: Shoot
- Space: Jump
- Shift: Sprint
- R: Reload
- Q: Swap weapon or mode

### Mobile

- Left joystick: Move
- Right-side fire button: Shoot
- Jump button: Jump
- Reload button: Reload
- Aim toggle or drag to look if enabled

## Gameplay Loop

1. Player spawns into the arena
2. Player moves and aims using their input device
3. Player fires a weapon
4. The server validates damage and hit targets
5. Health is reduced, and death triggers respawn
6. Match system tracks score, kills, and round state

## Core Design Principles

- Client handles input and visuals
- Server handles health, damage, and game state
- RemoteEvents are used for shooting and match updates
- Keep code modular and easy to expand

## Getting Started

1. Open Roblox Studio
2. Create a new place
3. Insert the scripts from the `scripts/` folders
4. Configure the arena map and spawn points
5. Test with PC controls first, then mobile controls
6. Add weapons, animations, and UI as you expand the project

## Beginner Tips

- Start with one weapon only
- Keep the map small and easy to navigate
- Use a single arena at first
- Validate damage on the server only
- Build mobile UI after PC gameplay feels solid

## Future Features

- Multiple weapons
- Bots or AI enemies
- Scoreboard and match timer
- Weapon recoil and spread
- Mobile-friendly HUD
- Round-based gameplay
- Leaderboards and progression

## License

This project is currently under a simple open-source setup for learning and prototyping. You can modify, extend, and build on it as needed.

## Notes

This repo is designed as a clean foundation for a Roblox FPS prototype, not a full commercial game. It is intentionally simple so new developers can learn the structure before adding advanced systems.

## Contributing

Feel free to fork the project, add improvements, and submit pull requests. The best additions are simple, readable, and game-focused.

## Example Project Name Ideas

- Roblox FPS Prototype
- Arena Strike
- Mobile FPS Arena
- Pixel Fire
- FPS Survival Demo

If you want, you can later rename the repo or turn this into a more specific game theme like sci-fi, military, or zombie FPS.
