# Resident Evil Village Archipelago (RE8 AP)

Client Archipelago for **Resident Evil Village**. Version **1.0.8**.

Site: https://lechapelierhd.github.io/Re8-AP-site/  
Releases: https://github.com/LechapelierHD/Re8-AP-site/releases

## Downloads

| File | Purpose |
|------|---------|
| [RE8_AP_Client_1.0.8.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.8/RE8_AP_Client_1.0.8.zip) | Launcher (single-file) + Lua + apworld |
| [REFramework_RE8_1.5.9.1.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.8/REFramework_RE8_1.5.9.1.zip) | REFramework separate |
| [RE8_AP_Bundle_1.0.8.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.8/RE8_AP_Bundle_1.0.8.zip) | Client + REFramework side by side |
| [re8ap_patch_1.0.8.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.8/re8ap_patch_1.0.8.zip) | Update patch (RE9-style) |

## Patch mechanic (like RE9)

- Launcher is **single-file self-contained** — « Mettre à jour » replaces the exe and restarts
- Each release hosts `patches.json` + `re8ap_patch_*.zip` via `publish_github.ps1`
- Drop a patch zip into the `Patchs` folder for offline install

## Antivirus

REFramework (`dinput8.dll`) is **not** inside the client zip.