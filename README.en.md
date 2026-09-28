# ScrapeFun Server for Windows

[简体中文](./README.md) · **English**

[Product overview](https://github.com/HaoweiLi97/ScrapeFun/blob/main/README.en.md) · [Stable downloads](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/latest) · [All releases](https://github.com/HaoweiLi97/scrapefun-server-windows/releases) · [Online documentation](https://scrapefun.com/?lang=en#/docs)

> Updated: 2026-09-28. Versions and assets below are the stable releases checked on this date. Follow the corresponding Release for later changes.

A Windows system-tray host with the ScrapeFun Server runtime and a management interface in your default browser. Manage movie, TV, comic, and remote WebDAV / AList libraries, and let Clients on your LAN connect.

## Downloads and environment

| Item | Current stable release |
| --- | --- |
| Version | [0.3.3](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/tag/v0.3.3) |
| Architecture | x64 |
| First installation | `ScrapeFunServer-stable-Setup.exe` |
| Update assets | `releases.stable.json`, `ScrapeFunServer-0.3.3-stable-full.nupkg` |

Download setup from the [stable download page](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/latest). Do not use nupkg for a first installation. System requirements and publisher signing status follow the actual installer and release information.

## Installation and first launch

1. Run setup, complete installation, and launch Server.
2. Open the ScrapeFun web interface from the system tray. The default address is `http://127.0.0.1:8096`.
3. For a new instance, follow the web setup to configure administrator credentials, storage, and libraries.
4. Enable LAN access and check the firewall when other devices need to connect.

Existing instances continue using their existing accounts. An older version's initial-password log workflow should not be assumed to apply to all new versions.

## System tray and data directory

The tray menu provides actions to open the web interface, restart the service, view data and logs, start with Windows, control LAN access, and check for updates.

Runtime data defaults to:

```text
%APPDATA%\ScrapeFunDesktop
```

Business data is in `data` and logs are in `logs`. These files live outside the installation directory; installer updates normally retain them. Deleting the user data directory affects the entire instance. Back up before doing so.

## Updates and migration from older installations

Velopack currently manages stable / beta updates. Check for updates in the web settings or tray, or run newer setup. Updates restart the service, so pause tasks and export a backup first.

For an older Inno Setup installation, exit and uninstall the old host, then run Velopack setup once. Retain `%APPDATA%\ScrapeFunDesktop` and check login, libraries, and data after migration. You can then use in-app updates.

## Troubleshooting

If the service cannot be opened, check processes, port conflicts, the log directory accessible from the tray, and the firewall. Reports should include Windows version, Server version, installation method, and logs with sensitive details removed.

## Support and licensing

This repository provides platform installation instructions and official release assets. Submit usage questions and feature requests to the [main repository Issues](https://github.com/HaoweiLi97/ScrapeFun/issues). For accounts, activation, or private logs, contact `scrapefun@outlook.com`. Report security issues privately according to the [security instructions](./SECURITY.en.md).

See the new [commercial license statement](./LICENSE.en.txt) and full [software license agreement](./EULA.en.md). Ordinary personal, household, and internal organizational use is allowed. Pro requires a valid entitlement. Software redistribution, resale, customer delivery, and paid hosting require separate written authorization. The statement does not retroactively change existing licenses; existing assets follow their supplied licenses, and third-party components retain their own licenses.

[Releases and compatibility](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.en.md) · [Third-party components](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.en.md) · [Support](./SUPPORT.en.md)
