# Manuk Shaolin Monks (MKSM Modloader for Android)

An unofficial native Android port of the original Xbox version of *Mortal Kombat: Shaolin Monks*, with a mod loader, Play As and extra options added by Manuk Bulan.

This is a fork of [**ShaolinMonks-Android**](https://github.com/RanggaCasper/ShaolinMonks-Android) by **Rangga Casper**. The port itself is his work: the game's x86 code is statically recompiled to C++ with [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp) and built for arm64. Vulkan does the drawing, and SDL3 handles the window, input and audio. No emulator is involved. What this fork adds is listed in [RELEASE_NOTES.md](RELEASE_NOTES.md).

> [!NOTE]
> This project does not include any game assets. You must provide the files from your own legally acquired copy of the game.

## Installation
1. Install the APK (Android 9 or newer, arm64, Vulkan 1.1).
2. Open **Manuk Shaolin Monks** and allow **all files access** when it asks (on Android 9 and 10, the **storage** permission).
3. Copy the game (the `.iso`, or `default.xbe` with the rest of the disc's files) into `ManukShaolinMonks/Game` on the phone's storage or SD card. The app creates the folders and starts the game once it finds the files.

| Folder | What goes there |
| --- | --- |
| `ManukShaolinMonks/Game` | the game files |
| `ManukShaolinMonks/Mods/Gamedata_wad` | mods (each mod in its own folder) |
| `ManukShaolinMonks/Savedata` | saves |
| `ManukShaolinMonks/crash_log.txt` | written after a crash; include it when you report a problem |

## Building
Building requires a Windows PC. Put `default.xbe` (or the `.iso`) in `assets/`, then run `build_release.bat`. On the first run it installs the Android SDK, NDK and CMake on the same drive as the project. The signed APK and the build logs go to `outputapk/`.

## Credits
- [ShaolinMonks-Android](https://github.com/RanggaCasper/ShaolinMonks-Android) and [Black-Android](https://github.com/RanggaCasper/Black-Android) by **Rangga Casper**: the original port and Android host.
- **Manuk Bulan**: the mod loader and the additions in this fork.
- [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp) by **TGP482**: the static recompiler and runtime.
- **Zukiru**: the HDR screen filter.
- **MustopuhGGI**: the MKSM character list.
- **OGMidway**: the tools reference.
- [SDL](https://github.com/libsdl-org/SDL), [glslang](https://github.com/KhronosGroup/glslang), [toml++](https://github.com/marzer/tomlplusplus), [Dear ImGui](https://github.com/ocornut/imgui), and [xemu](https://github.com/xemu-project/xemu) / [Cxbx-Reloaded](https://github.com/Cxbx-Reloaded/Cxbx-Reloaded) as references.

## Community
Mods, help and updates: the [ALL MODDING PS2/WII/XBOX GAME](https://t.me/manukbulanallmoddingameconsole) Telegram group.

## Support
- Rangga Casper: [SociaBuzz](https://sociabuzz.com/racas/tribe)
- Manuk Bulan: [Trakteer](https://trakteer.id/andriyanblaze/)

*Mortal Kombat* is a trademark of Warner Bros. Entertainment Inc. This project is not affiliated with or endorsed by them.
