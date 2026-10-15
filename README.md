# Call of Duty: Black Ops 2 — PS3 SPRX Mod Menus: The Definitive Guide

---

## Join Our Discord

- **Discord:** unosdopplegange
- **Discord server:** https://discord.gg/MDcaC5nPuA

> Research compiled 2026-10-10. Every menu below is a real, publicly-released SPRX (or SPRX loader/pack) for BO2 on PS3. Creators are credited. Compatibility is stated where it could be established; where it couldn't, it's marked unknown rather than guessed.

---

## Quick Facts

| Item | Detail |
|---|---|
| Game | Call of Duty: Black Ops 2 (Treyarch engine — **not** IW engine) |
| US Title ID | **BLUS31011** (disc) / **NPUB31054** (US PSN digital) |
| EU Title IDs | **BLES01717** (main EU), also BLES01718, BLES01719 |
| Final title update | **1.19** (confirmed; menus are built/targeted for 1.19) |
| SPRX install path | `dev_hdd0/tmp/` |
| Modded EBOOT path | `dev_hdd0/game/<TITLE_ID>/USRDIR/EBOOT.BIN` (or `t6mp_ps3f.self`) |
| Era | 2013–2017 peak; scene revival/porting activity ongoing (2020–2026) |

---

## How BO2 SPRX Menus Load

BO2 on PS3 has no unsigned-patch loophole. Menus load through a **modded EBOOT.BIN (or `t6mp_ps3f.self`)** with an SPRX loader baked in:

1. Copy the modded `EBOOT.BIN` (or `t6mp_ps3f.self`) to `dev_hdd0/game/<YOUR_REGION>/USRDIR/`, replacing the stock one.
2. Copy the `.sprx` file to `dev_hdd0/tmp/`.
3. Launch BO2 — the SPRX loads at game boot. Each menu has its own button combo (e.g. D-Pad Up + R3, L2 + Triangle, L1 + R3).

The **EBOOT must match your firmware type**: DEX EBOOTs need DEX CFW, CEX/HEN EBOOTs are signed differently. Using a DEX EBOOT on CEX (or vice versa) is the #1 reason a menu "doesn't work."

### Do SPRX menus need to match the installed TU?

Yes. SPRX menus are built against memory addresses for a specific title update. The BO2 scene standardized on **1.19** (the final TU), and nearly every menu listed here targets 1.19. If you're on an older TU, update the game to 1.19 first.

---

## GSC vs SPRX for BO2

BO2 supports **both**, which is why the scene is so big:

- **GSC menus** — script menus injected live via RTM tools (GSC Studio + CCAPI/TMAPI) or loaded from console by an **SPRX GSC injector** (e.g. `BO2_GSC_Injector.sprx`). Easier to write, host-only, and must be re-injected every session.
- **Native SPRX menus** — written in C++ against the PS3 SDK, these do things GSC cannot: **non-host/off-host aimbots, ESP/wallhacks, pre-game force-host, red boxes, VSAT** — the features that made BO2 menus famous. This is why the scene went SPRX: the competitive modding (aimbot/ESP) that defined BO2 *requires* native code.

Many releases bundle both: an SPRX injector that loads a set of GSC menus from `dev_hdd0/tmp/`.

---

## CFW vs HEN vs DEX/CEX Compatibility

- **The classic era (2013–2017) was DEX-dominant.** Most SPRX menus shipped with DEX EBOOTs and were tested on DEX CFW (Rebug DEX etc.). On CEX you need a CEX-signed EBOOT for the same SPRX — several releases include both.
- **HEN-compatible builds exist.** The standout is the **BO2 Lunar SPRX**, which ships separate **CFW and HEN** builds. The **100+ SPRX Mod Installer PKG** (Zeam, updated 2026) also ships separate DEX and HEN builds and installs 100+ SPRX menus BLES+BLUS.
- **CCAPI works on CEX; TMAPI is DEX-only.** RTM-based GSC injection needs one of them; native SPRX menus need neither once the EBOOT+SPRX are in place.
- **NPUB31054 (US digital)** — most SPRX menus are coded for BLUS/BLES memory layouts; digital-version users historically had trouble with off-host menus.

---

## Complete SPRX Menu Catalog

### Flagship / All-in-One SPRX Menus

#### Jiggy v4.x (v4.2 / v4.3 / v4.4)
- **Creator:** JiggyMods (credited as "Jiggymods" on release posts)
- **What it does:** One of the most famous BO2 menus ever — all-in-one host menu: god mode, unlimited ammo, UFO mode, fun mods, unique options. PS3 + Xbox 360.
- **Compatibility:** CFW (DEX-era release); TU 1.19
- **Source:** not public
- **Download:** CabConModding release thread (attachment `Jiggy 4.4.rar`) — https://cabconmodding.com/threads/jiggy-4-4-not-made-by-me.2684/
- **Status:** thread live; attachments on forum (login may be required)

#### Assassin v3.8 SPRX (Non-Host)
- **Creator:** release via ConsoleCrunch community
- **What it does:** Non-host SPRX with pre-game menu (force host, super force host, anti-freeze, name changer, recovery) + in-game menu (aimbot menu, fun options, user list, lobby info). Aimbot toggle shortcut.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** ConsoleCrunch thread — https://consolecrunch.com/threads/mod-menu-bo2-sprx-assassin-v3-8-new-update-spoof-ip-pre-game-non-host-1-19.28593/page-46
- **Status:** thread live (46+ pages); download link inside

#### Perplexed v4.2 SPRX (Non-Host)
- **Creator:** Perplexed team
- **What it does:** Non-host/off-host SPRX menu. One of the go-to off-host picks alongside Paradox.
- **Compatibility:** CFW (DEX EBOOT era); TU 1.19. Note: coded for BLUS/BLES, not NPUB31054 digital.
- **Source:** not public
- **Download:** Se7enSins mega-collection (see "Bulk packs" below)
- **Status:** available inside the Se7enSins PS3 mega collection

#### Paradox v2 / v3
- **Creator:** Paradox team
- **What it does:** All-in-one SPRX with a "beastly aimbot" per community reviews; got many players into non-host modding.
- **Compatibility:** CFW; TU 1.19. Coded for BLUS/BLES, not NPUB31054.
- **Source:** not public
- **Download:** CabConModding/NGU release threads (login-gated); also bundled in SPRX packs
- **Status:** release threads exist on NGU/CabCon (login required)

#### Trinity SPRX / Trinity Non Host v3.0
- **Creator:** Trinity team
- **What it does:** All-in-one SPRX; separate Non Host v3.0 build.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection; forum threads (login-gated)
- **Status:** in circulation

#### Profound V3 / V4
- **Creator:** Harry (CabConModding premium member; streamed the development)
- **What it does:** All-in-one SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** CabConModding release threads (login-gated)
- **Status:** threads live; noted community dispute about reused code, but release is real

#### Genisys V3.4
- **Creator:** Genisys team
- **What it does:** All-in-one SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection — https://www.se7ensins.com/forums/threads/release-ultimate-playstation-3-ps3-mod-menu-package-tools-mega-collection.1931291/
- **Status:** live thread, active as of 2026

#### Insomnia v2.1
- **Creator:** Insomnia team
- **What it does:** All-in-one SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Voltage
- **Creator:** Voltage team
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Anomaly SPRX
- **Creator:** Anomaly team
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Inception (BO2)
- **Creator:** Inception team
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Zodiac Framework V1
- **Creator:** SpikyCFW (credits: B777x, Shark, gopro_2027, Host Only, ix Skillz HD xi)
- **What it does:** SPRX framework/menu; v2.1 promised with better pre-game menu, scrollbar, scroller remembrance.
- **Compatibility:** CFW; TU 1.19; install: `dev_hdd0/Spiky` folder + EBOOT into game folder
- **Source:** not public
- **Download:** CabConModding thread — https://cabconmodding.com/threads/v1-of-zodiacframework-sprx.3123/
- **Status:** thread live

#### BO2 Lunar SPRX — **CFW and HEN builds**
- **Creator:** Lunar team
- **What it does:** All-in-one SPRX menu, notable for shipping **separate CFW and HEN builds** — one of the few BO2 menus with an explicit HEN variant.
- **Compatibility:** **CFW and HEN** (separate builds); TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Tempess CE (Premium Edition, 2020)
- **Creator:** released by Deno80 (ConsoleCrunch)
- **What it does:** Non-host mod menu; host can use god mode. New build as of 2020.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** ConsoleCrunch thread — https://consolecrunch.com/threads/bo2-sprx-tempess-ce-new-2020-non-host-mod-menu-premium-edition-host-can-using-god-mode.30228/ (Google Drive folder linked in thread)
- **Status:** thread live

#### BO2 Chickhen V2
- **Creator:** Chickhen team
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### BO2 Inphnect Pak
- **Creator:** Inphnect team
- **What it does:** SPRX menu pack.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### BO2 TS SPRX (by Zeam)
- **Creator:** Zeam
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Nexus_BO2_Crack
- **Creator:** Nexus team (cracked release)
- **What it does:** Cracked build of the Nexus BO2 SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public (crack of a paid/private menu)
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Reflex Engine V4 (Crack)
- **Creator:** Reflex team (cracked release)
- **What it does:** Cracked build of Reflex Engine V4 SPRX.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public (crack)
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Kebab Engine 1.5.2 (BO2 SPRX)
- **Creator:** Kebab team
- **What it does:** SPRX menu (Kebab Engine series spans BO1/BO2/BO3/AW).
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### BO2 Mary Jane
- **Creator:** Mary Jane team
- **What it does:** SPRX menu.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### BO2 THEE ANTICHEAT V1
- **Creator:** unknown
- **What it does:** Anti-cheat SPRX (server-side/lobby protection rather than a mod menu).
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** Se7enSins mega-collection (link above)
- **Status:** live

#### Bossam v5 / v6
- **Creator:** Bossam team
- **What it does:** All-in-one SPRX menu; v6 bundled in the Beast_Modz loader pack.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** CabConModding SPRX loader pack — https://cabconmodding.com/threads/bo2-sprx-loader-2-modmenus-and-21-custom-game-modes.2225/
- **Status:** thread live

#### Jericho Engine (Non-Host SPRX)
- **Creator:** ExiLe (Jericho Engine)
- **What it does:** One of the earliest-loved SPRX menus; non-host build available.
- **Compatibility:** CFW (DEX EBOOT); TU 1.19
- **Source:** not public
- **Download:** forum threads (Se7enSins/CabCon); non-host build in DEX 1.19 packs
- **Status:** in circulation

#### Revolution (SPRX version)
- **Creator:** Revolution team
- **What it does:** SPRX build (distinct from similarly-named RTM tools — community notes confirm the SPRX version is real).
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** forum threads (login-gated)
- **Status:** in circulation

#### Insidious
- **Creator:** Matrix
- **What it does:** SPRX menu with strong options and game modes.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** forum threads (login-gated)
- **Status:** in circulation

#### Lupos SPRX
- **Creator:** lupospmt809
- **What it does:** Small, simple BO2 (+ GTA) menu: UAV, red boxes, no blur, no recoil, body/map colors.
- **Compatibility:** CFW; TU 1.19
- **Source:** not public
- **Download:** CabConModding preview thread (BO2 section tag listing)
- **Status:** preview thread live; release small/early

---

### Non-Host / Off-Host SPRX Menus

These are the aimbot/ESP-capable menus that work without host — the core of BO2's SPRX reputation.

| Menu | Creator | Notes | Compatibility | Link / Status |
|---|---|---|---|---|
| YAE Non Host 1.5 | YAE team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Paradise Non Host v1.0 | Paradise team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Phoenix Host/Non-Host | Phoenix team | Host + non-host builds | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Arcadia Non Host v1.1 | Arcadia team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Non Host Complex v2.0 | Complex team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Lucid Non Host v2 | Lucid team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Suspected Engine (Non-Host) | Suspected team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| 4XC Non Host | 4XC team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Perxy Non Host v3.0 | Perxy team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| ProjectGT Non Host v2.0 | ProjectGT team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Stress (Non-Host) | Stress team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Exo Engine Non Host | Exo team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |
| Dex Fashions 1.19 | Fashions team | Non-host SPRX | CFW (DEX), 1.19 | DEX 1.19 mod packs (forum) |

> These non-host menus circulated mainly in DEX 1.19 compilation packs (e.g. the "BLUS31011-AUTO" style packs). They need a DEX EBOOT + DEX CFW.

---

### Zombies SPRX Menus

| Menu | Creator | Notes | Compatibility | Link / Status |
|---|---|---|---|---|
| Reincarnation (Zombies SPRX) | Reincarnation team | Zombies SPRX | CFW (DEX), 1.19 | DEX 1.19 packs; Se7enSins mega-collection |
| Extortion v1 (Zombies) | Extortion team | Zombies SPRX | CFW (DEX), 1.19 | DEX 1.19 packs; Se7enSins mega-collection |
| Liceme v1 (Zombies) | Liceme team | Zombies SPRX | CFW, 1.19 | Se7enSins mega-collection |
| Project Blue V2 (Zombies) | Project Blue team | Zombies SPRX | CFW, 1.19 | Se7enSins mega-collection |
| Zombies Escalation (CFW) | Escalation team | Zombies SPRX, CFW build | CFW, 1.19 | Se7enSins mega-collection |
| FENIX v5 (Zombies) | Fenix team | Zombies SPRX, well-regarded | CFW, 1.19 | YouTube showcases; forum threads |

---

### SPRX GSC Injectors & Loader Packs

#### BO2 GSC Injector SPRX (v1.1 / v1.7.5 / v2Beta)
- **Creator:** NzV (v1.1+; earlier builds associated with seriousHD)
- **What it does:** SPRX plugin that injects compiled GSC files into BO2 MP/Zombies on-console — no PC needed after setup. Loads `bo2_injector_path.txt` / `bo2_injector_file.gsc` from `dev_hdd0/tmp/` or USB.
- **Compatibility:** **CEX and DEX CFW** (no CCAPI needed); TU 1.19. Tested on Rebug Cobra 4.53.1.
- **Source:** not public
- **Download:** NGU release thread (login-gated) — https://nextgenupdate.com/forums/black-ops-2-mods-cheats-guides/773799-release-sprx-bo2-gsc-injector-v175-v2beta-13.html
- **Status:** thread live; downloads login-gated

#### GSC Injector v2.32
- **Creator:** unknown (French modding scene)
- **What it does:** SPRX GSC injector bundled in DEX 1.19 packs.
- **Compatibility:** CFW (DEX), 1.19
- **Source:** not public
- **Download:** DEX 1.19 compilation packs
- **Status:** in circulation

#### BO2 SPRX Ultimate Injector V2.4 (GfK)
- **Creator:** GfK (AsO GaMeR release post)
- **What it does:** Multi-menu SPRX injector — 12 mod menus (Dynamic V3.3, Radiant V1.5.1, Bossam V5/V6, Jiggy V4.2, Foundalized V1, Acid Rain V2.6, Elegance V5 Lite, oCmKs_4_LiFe's Private Menu, Inspire V1, Predator V5.3, Azza V2) + 8 game modes. Open with L2+R2+Triangle (lobby only).
- **Compatibility:** CFW; 1.19
- **Source:** not public
- **Download:** NGU thread (login-gated) — https://nextgenupdate.com/forums/black-ops-2-gsc-mods-scripts/932015-bo2-sprx-new-update-gfksprxbo2menus-ultimate-sprx-injector-v24a.html
- **Status:** thread live; downloads login-gated

#### philwill123's SPRX GSC Injector Pack (10 ModMenus)
- **Creator:** philwill123 (pack; menus by their authors)
- **What it does:** SPRX injector pack: White Water V5.5, Dynamic V2.2, Game Mode Loader, Caked UP V1.8, BossamV2, Gr3Zz v4.0 Zombie Patch, Red Tear, Silent Shadow, Elegance V2.4, Elegance V3.
- **Compatibility:** CFW; 1.19/2.19
- **Source:** n/a (pack)
- **Download:** NGU thread (login-gated) — https://nextgenupdate.com/forums/black-ops-2-gsc-mods-scripts/818265-ps3-bo2-119219-sprx-gsc-injector-10-modmenus-2.html
- **Status:** thread live; downloads login-gated

#### Beast_Modz SPRX Loader (2 modmenus + 21 custom game modes)
- **Creator:** Markf2015 (pack; menus by their authors)
- **What it does:** SPRX loader bundling Bossam v6, Jiggy v4.2 + 21 custom game modes (Prop Hunt, Floor is Lava, Mario Kart, etc.).
- **Compatibility:** CFW; 1.19
- **Source:** n/a (pack)
- **Download:** CabConModding thread — https://cabconmodding.com/threads/bo2-sprx-loader-2-modmenus-and-21-custom-game-modes.2225/
- **Status:** thread live with attachment

---

### Bulk Packs (the easy way to get everything)

#### Se7enSins Ultimate PS3 Mod Menu/Package/Tools Mega Collection
- **What it is:** Active (2026) mega-thread with 20+ BO2 SPRX menus: Anomaly, Chickhen V2, Extortion v1 Zombies, Genisys V3.4, Inception, Inphnect Pak, Insomnia v2.1, Liceme v1 Zombies, **Lunar CFW + Lunar HEN**, Mary Jane, Project Blue V2 Zombies, Reincarnation Zombies, THEE ANTICHEAT V1, TS SPRX by Zeam, Zombies Escalation (CFW), Kebab Engine 1.5.2, Nexus_BO2_Crack, Perplexed, Reflex Engine V4 Crack, Voltage, Zodiac Framework — plus BO1/BO3/AW/MW menus and tools.
- **Link:** https://www.se7ensins.com/forums/threads/release-ultimate-playstation-3-ps3-mod-menu-package-tools-mega-collection.1931291/
- **Status:** live and updated; free leech

#### 100+ SPRX Mod Installer PKG (CFW/HEN) by Zeam
- **What it is:** PS4-themed PKG installer with 100+ SPRX menus (BLES+BLUS), **separate DEX and HEN builds** (updated 2026). Easiest path to SPRX menus on HEN.
- **Creator:** Zeam (packager); menus by their authors
- **Link:** YouTube showcase — https://www.youtube.com/watch?v=gKpFuDtXtDc (MediaFire links in description)
- **Status:** video live; MediaFire links as of 2026

---

### Open-Source BO2 SPRX Projects (GitHub)

| Project | Author | What it is | Link |
|---|---|---|---|
| Synapse BO2 SPRX Menu Base | horrortify | C++ PS3 PRX menu base (Stanky-style UI, R3+L1 open, god mode/UAV/laser/red boxes, host detection) | https://github.com/horrortify/synapse-bo2-sprx-base |
| DeadOps | ItsJokerZz | GSC-loader SPRX for PS4/PS5 that runs BO2 GSC scripts (t6mp/t6zm) — relevant for porting BO2 menus forward | https://github.com/ItsJokerZz/DeadOps |

**Login-gated open bases (NGU, free account):**
- **oStankyModz BO2 Ultimate Menu Base [SPRX/C++]** — full SPRX/C++ base, CEX+DEX EBOOTs included. Credits: Seb5594 (TOC), Shark (button monitoring). Built with Visual Studio 2010 + PS3 SDK. https://nextgenupdate.com/forums/black-ops-2-mods-cheats-guides/773122-release-bo2-ultimate-menu-base-sprxc-2.html
- **RTE's BO2 Zombie SPRX Menu Base [1.19]** — zombie-mode SPRX base. Credits: Seb5594 (TOC), Shark (HUDs). https://nextgenupdate.com/forums/black-ops-2-mods-cheats-guides/796993-release-bo2-zombie-sprx-menu-base-119a.html

---

## RTM Tools for BO2 (PC-side)

These connect over CCAPI (CEX) or TMAPI (DEX) for live memory editing and GSC injection:

| Tool | Creator | Features | Notes |
|---|---|---|---|
| GSC Studio | iMCSx (French Modding Team) | Write/compile/inject GSC menus live; the standard BO2 GSC workflow | NGU thread; CCAPI 2.60 era |
| Project TCM Injector | Project TCM team | GSC injector, CCAPI 2.60 | ConsoleCrunch thread; "biggest menu" (1500+ options) |
| ExIIL Multi COD RTM + Debugger | ExIIL | Multi-CoD RTM tool incl. BO2 | CCAPI/TMAPI |
| RTM Tool (BO2) | Geo | BO2 RTM | CCAPI 2.60 |
| League Play RTM Tool | iJosh | BO2 league play RTM | CCAPI 2.60 |
| RTM Tool (BO2) | ITz_JeWeLs | BO2 RTM | CCAPI 2.60 |
| RTM Tool (BO2) | One | BO2 RTM | CCAPI 2.50/2.60 |
| Zombies RTM Tool | SKush420 | BO2 zombies RTM | CCAPI 2.50/2.60 |
| RTM Tool (BO2) | Stunz | BO2 RTM | CCAPI 2.50/2.60 |
| Kiwi Mods RTM | Kiwi | Multi-CoD RTM | Community-noted as clean/safe build |
| NetCheat | — | Memory debugger | Used for BO2 offset work |
| 444xMoDz RTM tools | 444xMoDz | MW2/MW3/BO2 RTM | NGU |

**Companion EBOOTs (NGU Supreme Modding Guide):** ITz_JeWeLs' CEX/DEX EBOOTs (antiban, laser, VSAT, red boxes, no recoil), B777x's DEX EBOOT (non-host aimbot, VSAT, red boxes, anti-freeze) — https://nextgenupdate.com/forums/black-ops-2-mods-cheats-guides/798649-black-ops-2-supreme-modding-guide-eboots-tools-pkg-files-gsc-23.html (login-gated)

---

## How They Were Built

- **Toolchain:** Sony PS3 SDK + **Visual Studio 2010 Ultimate** (per oStankyModz's release notes) — the standard for the era.
- **Key community contributions reused everywhere:** **Seb5594's** TOC addresses, **Shark's** button-monitoring/HUD code, NGU offset threads.
- **Why SPRX won on BO2:** Treyarch's engine + the 1.19 TU made native C++ menus the only way to get non-host aimbots, ESP, and pre-game force-host. GSC stayed popular for host lobbies (easier to write, injectable via GSC Studio), but every competitive/off-host feature in this catalog is native SPRX.
- **TU targeting:** menus hardcode 1.19 addresses; the EBOOT loader + SPRX in `dev_hdd0/tmp/` pattern was universal.

---

## Names I Could NOT Verify as BO2 PS3 SPRX Menus

The seed list included several names I could not confirm as real BO2 *PS3 SPRX* releases after deep searching (they may be Xbox 360 menus, menus for other CoDs, GSC-only, or misremembered names): **Envy, Exotic, Element, xAzt3c, Swaqqin, Apocalypse, Fatality** (known as a BO3 menu by Enstone), **Reborn, Extinct, Venom, Toxic, Chaos, Oblivion** (known on AW), **xC4, xKiller, xLithium, Destruction, Echelon**. If you have a link for any of these as a BO2 PS3 SPRX, it belongs in this catalog — open an issue/PR.

---

## Sources

- Se7enSins — Ultimate PS3 Mod Menu/Package/Tools Mega Collection (2026)
- CabConModding — BO2 mods section (Jiggy 4.4, Zodiac Framework, Beast_Modz loader, BO2 modding guide)
- NextGenUpdate — BO2 SPRX releases (GSC Injector v1.7.5, Ultimate Injector V2.4, 10-menu pack, oStankyModz base, RTE zombie base, Supreme Modding Guide)
- ConsoleCrunch — Assassin v3.8 SPRX, Tempess CE threads
- setsid/ps3-tools (GitHub) — hardware-verified BLES01717 TU 1.19
- GitHub — horrortify/synapse-bo2-sprx-base, ItsJokerZz/DeadOps
- YouTube — Zeam 100+ SPRX Mod Installer PKG showcase (2026)

---

*Guide for Richard's BO2 SPRX repo. Menus are listed with creators credited; nothing here is claimed to work until tested on real hardware.*
