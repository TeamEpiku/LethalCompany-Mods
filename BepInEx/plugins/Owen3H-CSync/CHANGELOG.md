## v1.0.7
- Fixed syncing issue when the host's game path was not the same as the client's.
- Caching now uses the file name instead of the absolute path.
- When calling `SyncInstance`, the `Synced` bool is now set according to whether deserialization succeeds.

## v1.0.6
- Removed the type constraint from `SyncedEntry` to fix an error when using the `string` type.
- Publicized the underlying `ConfigEntry` (named 'Entry') to enable compatibility with **LethalConfig**.
- Some small but important changes to `SyncedConfig`. It is still advised NOT to use this *yet*.

## v1.0.5
- The library is now available on **NuGet**.

## v1.0.4
- Minor edits to Thunderstore metadata. (No need to download this version)

## v1.0.3
- Implemented a config file cache to speed up deserialization of `SyncedEntry`'s.
- Exposed `BoxedValue` and `SettingChanged` from the underlying entry to `SyncedEntry` itself.
- Constrained the `SyncedEntry` type parameter to a primitive value.
- Added some documentation to classes.

## v1.0.2
- Fixed bug introduced in v1.0.1 causing syncing issues.
- Added a class constraint to the `SyncedInstance` type parameter.

## v1.0.1
- Renamed the built-in `SyncedConfig` to prevent confusion with the wiki.
- Reduced instance size by marking some internally used props as `[NonSerializable]`.
- Removed `Instance` property from the `CSync.cs` file as it's not necessary.

## v1.0.0
- Implemented `SyncedEntry` - a serializable alternative to `ConfigEntry`.
- Implemented `SyncedInstance` that aids with syncing and reverting.
- Implemented `ByteSerializer` to serialize instances with `DataContractSerializer`.
- Provided extension methods to `ConfigFile` and `FastBufferWriter`.