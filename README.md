# MyDMX

DMX lighting console for macOS and Windows: fixture patching, cues, effects, 3D visualizer, USB DMX interfaces (Enttec, DMXking) and MIDI control.

## Download

Get the latest installer from the **[Releases page](https://github.com/drtechsys/mydmx-releases/releases/latest)**:

| Your computer | Download |
|---|---|
| Mac with Apple Silicon (M1/M2/M3/M4) | `MyDMX-<version>-arm64.dmg` |
| Mac with Intel processor | `MyDMX-<version>.dmg` |
| Windows 10/11 (64-bit) | `MyDMX.Setup.<version>.exe` |

Not sure which Mac you have? Apple menu → **About This Mac**: "Chip: Apple M…" means Apple Silicon; "Processor: Intel" means Intel.

## Install

The installers are not yet code-signed, so your computer shows a warning the first time.

### macOS
1. Open the `.dmg` and drag **MyDMX** into **Applications**.
2. Open MyDMX. macOS will say it can't verify the developer — click **Done**.
3. Go to **System Settings → Privacy & Security**, scroll down and click **Open Anyway** next to MyDMX, then confirm.

You only need to do this once.

**If macOS says "MyDMX is damaged and can't be opened"**: click **Cancel** (not Move to Trash), make sure MyDMX is in Applications, then open **Terminal** and run:

```bash
xattr -cr /Applications/MyDMX.app
```

Then open MyDMX again. (This affected v1.0.2 and earlier; v1.0.3+ shouldn't need it.)

### Windows
1. Run `MyDMX.Setup.<version>.exe`.
2. If you see "Windows protected your PC", click **More info → Run anyway**.
3. Choose an install folder and finish the installer.

## USB DMX interfaces

FTDI-based interfaces (Enttec Open DMX / DMX USB Pro, DMXking ultraDMX) normally work without extra drivers. If Windows doesn't list the port, install the [FTDI VCP driver](https://ftdichip.com/drivers/vcp-drivers/).

## Credits

Fixture library from the [Open Fixture Library](https://open-fixture-library.org) (MIT). Fixture profiles: Powered by GDTF.

---

This repository only hosts release downloads.
