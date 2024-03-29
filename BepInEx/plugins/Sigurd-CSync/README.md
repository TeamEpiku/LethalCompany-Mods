# CSync [<img align="right" width="128" height="128" src="https://github.com/lc-sigurd/CSync/raw/main/CSync/assets/icons/icon.png">](https://thunderstore.io/c/lethal-company/p/Sigurd/CSync/)

[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/lc-sigurd/CSync/build.yml?style=for-the-badge&logo=github)](https://github.com/lc-sigurd/CSync/actions/workflows/build.yml)
[![Release Version](https://img.shields.io/github/v/release/lc-sigurd/CSync?style=for-the-badge&logo=github)](https://github.com/lc-sigurd/CSync/releases)
[![Thunderstore Version](https://img.shields.io/thunderstore/v/Sigurd/CSync?style=for-the-badge&logo=thunderstore&logoColor=white)](https://thunderstore.io/c/lethal-company/p/Sigurd/CSync/)
[![Thunderstore Downloads](https://img.shields.io/thunderstore/dt/Sigurd/CSync?style=for-the-badge&logo=thunderstore&logoColor=white)](https://thunderstore.io/c/lethal-company/p/Sigurd/CSync/)

A BepInEx configuration file syncing library.
This library will help you force clients to have the same settings as the host!

> [!IMPORTANT]
> - This is **NOT** a standalone mod, it is intended for mod developers and does nothing on its own!<br>
> - This does **NOT** edit or replace config files directly, everything is done in-memory.<br>
> - It will **NOT** sync configs from mods that aren't dependent upon it.<br>
> - CSync uses Unity's Named Messages to avoid **Netcode Patcher** and **NetworkBehaviour**.

## Disclaimer

This project is a **fork** of the [original CSync project](https://github.com/Owen3H/CSync) authored by
[@Owen3H](https://github.com/Owen3H).

## Features
- Can serialize a `ConfigEntry` with a drop-in replacement. (`SyncedEntry`)
- No seperate config file system, retains BepInEx support.
- Uses `DataContractSerializer`, a fast and safer alternative to `BinaryFormatter`.
- Provides helpful extension methods.

## Setup & Usage
A guide to both setting up and using CSync is available on [Lethal Wiki](https://lethal.wiki/dev/apis/csync).

## License
This project has the `CC BY-NC-SA 4.0` license.<br>
This means the following terms apply:

**Attribution**<br>
If you remix or adapt this project, appropriate credit must be given.<br>
Cloning the repo with intent to contribute is not subject to this.

**NonCommercial**<br>
You may not use this material for commercial purposes.

**ShareAlike**<br>
When remixing, adapting or building upon this material, you must
distribute the new material under the same license as the original.
