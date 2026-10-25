# buildxstudio.ai — Releases

Windows installers for **buildxstudio.ai**: design a home from a description or bring its drawings,
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

## Install

1. Download `buildxstudio-Setup-<version>.exe` and run it (Windows 10 or 11, 64-bit).
2. Windows may show *"Windows protected your PC"* because the installer is not code-signed yet:
   click **More info → Run anyway**.
3. Keep the PC online during the install: the optional DWG support and photoreal renderer
   (Blender, ~400 MB) are downloaded while installing. No administrator rights are needed.
4. Start **buildxstudio.ai** from the desktop or Start menu. It opens in your browser; keep its window
   open while you work. Demo projects are ready on the Projects page.

Silent install for IT: `buildxstudio-Setup-<version>.exe /S` (add `/NODOWNLOADS` to skip Blender and DWG support).

Projects are stored in `%LOCALAPPDATA%\buildxstudio.ai`; uninstall from Windows Settings → Apps.
