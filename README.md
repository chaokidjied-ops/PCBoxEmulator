# PC Box Emulator

Android launcher project targeting Counter-Strike 1.6 on ARM64 devices.

## Current scope
- First supported game: Counter-Strike 1.6 only.
- Target device for compatibility checks: Xiaomi Redmi A3x (3 GB RAM).
- Landscape-first interface with configurable touch controls.
- Keyboard and mouse input support.
- Game data is user-supplied; this repository does not distribute proprietary game assets.

## Engine integration
The intended native stack is:
- [Xash3D FWGS](https://github.com/FWGS/xash3d-fwgs) as the GoldSrc engine.
- [CS16Client](https://github.com/FWGS/cs16-client) as the Counter-Strike client/game code.

These projects have their own Android build systems and dependency requirements. Integration must preserve their licenses and upstream notices. A successful build alone does not prove the game starts: runtime testing with legally obtained `valve` and `cstrike` data is still required.

## Build status
This repository is an integration workspace. It is not yet a completed launcher, and no tested APK is published yet.

## Planned milestones
1. Reproducible ARM64 Android build of the upstream engine/client.
2. Android host application and storage access for user-provided game data.
3. Touch overlay wired to actual engine input.
4. Hardware keyboard and mouse handling.
5. APK build, install, and runtime validation on the target phone.

## Legal note
Obtain Counter-Strike 1.6 game data from a legitimate copy. Do not upload proprietary game archives to this repository.
