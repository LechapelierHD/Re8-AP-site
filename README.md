# Resident Evil Village Archipelago (RE8 AP)

Archipelago randomizer client for **Resident Evil Village** (Steam).  
Game name in Archipelago: `Resident Evil Village`  
Current client version: **1.0.4**

Site: https://lechapelierhd.github.io/Re8-AP-site/  
Releases: https://github.com/LechapelierHD/Re8-AP-site/releases

---

## What this mod does

- Turns item pickups into **Archipelago checks** (Village campaign).
- Shuffles (optional) **key items** with logic that avoids softlocks.
- Supports **Duke shop** checks, **hunting** meat checks, **boss rewards**, **Death Link**.
- Goals: end of game (Mother Miranda), four Lords, or a single Lord.
- Missable / point-of-no-return areas: excluded, auto-send, or 100% walls.
- In-game UI via REFramework (**Insert**): Connection, checks, guidance, hints, help.

---

## Requirements

1. **Resident Evil Village** (Steam)
2. **Archipelago** 0.6.8 (or compatible) to generate / host
3. **REFramework** for RE8 (downloaded by the launcher from the official nightly)

---

## Install (player)

1. Install **Resident Evil Village** on Steam.
2. Download **RE8_AP_Client_1.0.4.zip** from the [latest release](https://github.com/LechapelierHD/Re8-AP-site/releases/tag/v1.0.4).
3. Extract the folder `RE Village Archipelago` anywhere (Desktop is fine).
4. Run `RE8.AP.Launcher.exe`.
5. Open **Setup status**:
   - Set / detect the game folder (`re8.exe`).
   - Click **Install REFramework** (downloads official `RE8.zip` nightly → `dinput8.dll` next to `re8.exe`).
   - Install the Archipelago client scripts into the game.
6. **Join a multiworld**:
   - Configure your YAML (slot name, difficulty, key items, Duke shop, hunting, goal…).
   - Send the YAML to the host (or host yourself).
   - Enter room address / slot / password → **Install and join**.
7. Launch the game from Steam. Wait for the **connected** notification before picking items up.
8. **Insert** opens the RE Village Archipelago window (Connection tab if needed).

> `dinput8.dll` is **not** shipped in the client zip (antivirus false positives).  
> Use **Setup status → Install REFramework**, or grab [`RE8.zip`](https://github.com/praydog/REFramework-nightly/releases) yourself.

---

## Host / generate

1. Install Archipelago **0.6.8**.
2. Put `residentevilvillage.apworld` in Archipelago `custom_worlds`  
   (from the client package `assets/Data/`, or from **RE8_AP_Source**).
3. Collect player YAMLs (game must be `Resident Evil Village`).
4. Generate with Archipelago Generate, then host / open the room as usual.
5. Players join with the room address in the launcher (or in-game Connection tab).

---

## Downloads

| File | Purpose |
|------|---------|
| [RE8_AP_Client_1.0.4.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.4/RE8_AP_Client_1.0.4.zip) | Launcher + Lua client + apworld (no bundled `dinput8.dll`) |
| [RE8_AP_Source_1.0.4.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.4/RE8_AP_Source_1.0.4.zip) | Full source (apworld Python, Lua client, launcher C#) |
| [re8ap_patch_1.0.4.zip](https://github.com/LechapelierHD/Re8-AP-site/releases/download/v1.0.4/re8ap_patch_1.0.4.zip) | Update patch for an existing install (Updates tab / `Patchs` folder) |

---

## Main YAML options (summary)

| Option | Role |
|--------|------|
| `goal` | Victory: end of game, four Lords, or one Lord |
| `difficulty` | Required in-game difficulty (`au_choix` / casual / standard / hardcore / village of shadows) |
| `key_items` | Vanilla / shuffle in zone / zone or multiworld |
| `missable_checks` | Excluded / auto-send / 100% |
| `duke_shop` | Vanilla / unique items / unique + case upgrades |
| `hunting` | % of meat pickups that are checks (0–100) |
| `boss_rewards` | Extra boss treasure checks |
| `death_link` | Shared deaths |

Use the launcher **Join** flow to build a valid YAML without editing by hand.

---

## Antivirus / SmartScreen

Windows may still warn on first download: the launcher is **unsigned**.  
`dinput8.dll` is no longer inside the client zip — the launcher fetches it from [praydog’s nightly](https://github.com/praydog/REFramework-nightly/releases) when you click **Install REFramework**. Prefer the official GitHub release.

---

## Bugs

Post on the community hub: https://lechapelierhd.github.io/synthetic-shores/  

If possible, attach:

- `reframework/data/re_village_ap_client/debug_log.txt`
- `re2_framework_log.txt` (lines with `[RE Village AP]`)

You can also use **Generate bug report** in the launcher.

---

## License / credits

- Powered by [Archipelago](https://archipelago.gg/) and [REFramework](https://github.com/praydog/REFramework).
- Resident Evil Village © Capcom. This project is a fan randomizer client, not affiliated with Capcom.
