# decomp-registry

> Project-R decompilation and emulator fork registry — JSON database of known decompilation projects and game-specific emulator forks.

**Status:** Active · [Contributing Guide](CONTRIBUTING.md)

## Files

| File | Purpose |
|---|---|
| `decomp_registry.json` | Maps ROM MD5 hashes to decompilation projects |
| `emu_forks_registry.json` | Maps game IDs to game-specific ShadPS4/KytyPS5 forks |

## decomp_registry.json format

```json
{
  "rom_hash_md5": "20b854b239203baf6c961b850a4a51a2",
  "project_id": "sm64-us",
  "display_name": "Super Mario 64 (US)",
  "repo": "https://github.com/sm64pc/sm64ex",
  "build_system": "make",
  "deps": ["python", "audiofile", "sdl2"],
  "output_binary": "build/us_pc/sm64.us.f3dex2e"
}
```

## emu_forks_registry.json format

```json
{
  "emulator": "shadps4",
  "game_id": "CUSA00832",
  "display_name": "Bloodborne",
  "fork_repo": "https://github.com/shadps4-compat/shadps4-bloodborne",
  "stability": "stable",
  "notes": "Patches shader compilation for Bloodborne's specific GPU usage patterns"
}
```

`stability` must be `"stable"` or `"experimental"`.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

GPL-3.0
