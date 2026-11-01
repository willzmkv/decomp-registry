# Contributing to decomp-registry

## Adding a decompilation entry

1. Find the ROM MD5: `md5sum your-rom.z64`
2. Verify the decompilation project builds cleanly on Arch Linux
3. Add an entry to `decomp_registry.json` following the schema
4. Submit a PR

## Adding an emulator fork entry

1. Verify the fork exists and is actively maintained
2. Set `stability` to `"experimental"` unless the fork has been stable for 3+ months
3. Add an entry to `emu_forks_registry.json`
4. Submit a PR

## Supported emulators for emu_forks_registry

- `shadps4` — ShadPS4 (PS4)
- `kytyps5` — KytyPS5 (PS5)
