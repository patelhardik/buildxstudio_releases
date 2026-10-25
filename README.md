# buildxstudio.ai — Releases

Installers for **buildxstudio.ai** (Windows and Linux): design a home from a description or bring its drawings,
and get a material take-off, cost estimate, photoreal 3D renderings, construction drawings and
trade bid packages.

**Download:** see [Releases](https://github.com/patelhardik/buildxstudio_releases/releases).

## Beta and stable versions

* **Beta** versions (for example `0.1-beta`) are marked **Pre-release**. They have the newest
  features for early testing; some may change or not be finished yet. Please report anything that
  does not work.
* **Stable** versions (for example `0.1`) are marked **Latest** and are the ones to use for client work.

Installing a newer version over an older one keeps your projects. You can move between beta and
stable the same way: run the other installer.

| Platform | Download |
|---|---|
| Windows 10 / 11 (64-bit) | `buildxstudio-Setup-<version>.exe` |
| Ubuntu 22.04+ / Debian 12+ (64-bit) | `buildxstudio_<version>_amd64.deb` |
| macOS | coming in a later beta |

## Install on Windows

1. Download `buildxstudio-Setup-<version>.exe` and run it (Windows 10 or 11, 64-bit).
2. Windows may show *"Windows protected your PC"* because the installer is not code-signed yet:
   click **More info → Run anyway**.
3. Keep the PC online during the install: the optional DWG support and photoreal renderer
   (Blender, ~400 MB) are downloaded while installing. No administrator rights are needed.
4. Start **buildxstudio.ai** from the desktop or Start menu. It opens in your browser; keep its window
   open while you work. Demo projects are ready on the Projects page.

Silent install for IT: `buildxstudio-Setup-<version>.exe /S` (add `/NODOWNLOADS` to skip Blender and DWG support).

Projects are stored in `%LOCALAPPDATA%\buildxstudio.ai`; uninstall from Windows Settings → Apps.

## Install on Linux (Ubuntu / Debian)

1. Download `buildxstudio_<version>_amd64.deb`.
2. Install it from a terminal in the download folder (it asks for your password and adds the few system
   libraries it needs):
   ```bash
   sudo apt install ./buildxstudio_<version>_amd64.deb
   ```
   Keep the computer online: Blender (~350 MB, for photoreal renders) and the render textures are downloaded
   while installing. `sudo BXS_NO_DOWNLOADS=1 apt install ./buildxstudio_<version>_amd64.deb` skips them.
3. Start **buildxstudio.ai** from the applications menu (or run `buildxstudio`). It opens in your browser; keep
   its terminal window open while you work. Demo projects are ready on the Projects page.

Projects are stored in `~/.local/share/buildxstudio.ai`; uninstall with `sudo apt remove buildxstudio` (your
projects are kept). DWG drawings are not read on Linux yet: export them to PDF or DXF first.
