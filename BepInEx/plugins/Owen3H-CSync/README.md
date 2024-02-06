# CSync
A BepInEx configuration file syncing library.<br>
This library will help you force clients to have the same settings as the host!

Refer to the wiki for a usage guide.

## Features
- Can serialize a `ConfigEntry` with a drop-in replacement.
- No seperate config file system, retains BepInEx support.
- Uses `DataContractSerializer`, a fast and safer alternative to `BinaryFormatter`.
- Provides helpful extension methods.

## Setup
1. Download and extract BepInEx v5 into your game directory.
2. Extract the zip into your game directory root.
3. In your mod's project, add an **Assembly Reference** to `../BepInEx/plugins/CSync.dll`.

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
