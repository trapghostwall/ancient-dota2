# Troubleshooting

This page covers documentation and environment problems. Ancient does not
ship a loader, DLL, or executable, so there is no in-repo runtime to debug.

## The archive will not open

- Re-download once from the linked folder.
- Confirm the password exactly: `5139237619`.
- Try a current archive tool; old extractors may not support the compression.
- Check free disk space and the destination path length.
- If the archive is still broken, do not use a random mirror. Open an issue.

## The password is rejected

- Remove a trailing space from the copied password.
- Do not include quotes unless the vendor explicitly requires them.
- Confirm that Caps Lock and the keyboard layout are correct.
- If the file is a reupload, discard it and use the linked folder.

## The overlay does not appear

1. Close other overlays: Discord, GeForce Experience, OBS, RTSS, and recording
   tools can compete for the same graphics hook.
2. Switch Dota 2 to windowed borderless.
3. Match the game and desktop resolutions.
4. Restart the game before restarting the external tool.
5. Test without the external tool to confirm the game itself is healthy.

This repository cannot verify the overlay behavior of a third-party package.

## The game crashes on launch

- Remove the external tool from the process.
- Verify Dota 2 files through Steam.
- Update the GPU driver only after recording the current version.
- Disable one overlay at a time; do not change five variables at once.
- If the crash began after an update, restore the previous known-good setup.

## A configuration change does not persist

- Check whether the tool stores configs in its own folder or in `%APPDATA%`.
- Run the tool from a folder your user account can write to.
- Avoid a read-only or synced folder for active configs.
- Export the profile before editing it by hand.
- Check for two copies of the tool writing to the same config.

## Antivirus flags the download

Do not disable antivirus to force a download. A detection can be a false
positive, but it can also be correct. Upload the file to a reputable multi-engine
scanner, compare the hash with the vendor's published value, and ask the vendor
for a signed build. If those steps are not possible, do not run it.

## High frame-time or stutter

- Close recording and browser software.
- Test one overlay module at a time.
- Lower overlay scale or refresh rate.
- Revert the latest GPU driver if the stutter started with it.
- Compare frame time, not only average FPS.

## Permission errors

- Keep the tool outside `Program Files` and the Steam library.
- Use a normal user folder such as `D:\Tools\Ancient`.
- Avoid running as administrator unless the vendor documents a reason.
- Check that the folder is not controlled by a sync client or antivirus lock.

## Reporting an issue

Include the page, step, game build, Windows version, GPU driver, and a redacted
error message. Never post passwords, tokens, or account identifiers.

## Related pages

- [Installation](installation.md)
- [Configuration](configuration.md)
- [Safety](safety.md)
