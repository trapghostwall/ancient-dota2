# Configuration notes

Ancient documents configuration hygiene for Dota 2 companion tools. The
repository does not ship a config parser, executable, or game hook.

## Profiles

Use one profile per situation instead of one giant config:

| Profile | Purpose |
| --- | --- |
| Desktop | Native resolution, normal HUD scale |
| Laptop | Lower resolution, larger overlay text |
| Tournament | Minimal visuals, no experimental modules |
| Test | New settings that have not been validated yet |

Name profiles predictably, for example `desktop-1080p`, `laptop-1440p`, and
`test-2026-10`. A predictable name makes rollback and bug reports much easier.

## Backups

- Export the config before every update.
- Keep at least two known-good backups.
- Store backups outside the tool folder.
- Add a date and a short note to each backup.
- Do not sync a config folder that contains credentials or session tokens.

A simple backup convention:

```text
backups/
  2026-10-31_before-update/
  2026-10-24_known-good/
  2026-10-17_first-install/
```

## Display and overlay settings

- Windowed borderless is the safest starting point for overlay concepts.
- Match the game resolution and the desktop resolution before changing HUD scale.
- Increase text size before increasing panel density.
- Disable unused modules when measuring performance.
- Test at the lowest frame rate you normally accept, not only at maximum FPS.

## Hotkeys

- Avoid keys that Dota 2 already uses for abilities, items, camera, or chat.
- Do not bind a toggle to a key you press during a fight.
- Keep a visible reminder of the active profile.
- Test hotkeys in a lobby or demo, not in a ranked match.
- Document every custom binding in your own notes.

## Configuration files are untrusted input

Public configs can contain malformed values, unexpected paths, or references to
modules that do not exist. Inspect a config before loading it. Prefer a minimal
profile that you created yourself over a large config from an unknown source.

## Privacy

- Do not put Steam credentials in a config.
- Do not put API keys, webhook URLs, or tokens in a config.
- Do not publish logs that contain account names or session identifiers.
- Redact local paths before opening a public issue.

## Performance checklist

1. Close browser tabs and recording software before measuring.
2. Test one change at a time.
3. Record average frame time, not only peak FPS.
4. Revert the change if frame pacing gets worse.
5. Keep a stable profile available at all times.

## Related pages

- [Installation](installation.md)
- [Troubleshooting](troubleshooting.md)
- [Safety](safety.md)
