<p align="center"><img src="logo.png" alt="VN Deck" width="420"></p>

# VN Deck

A library and launcher for visual novels you download yourself, from itch.io, F95zone and anywhere else. Ren'Py, RPG Maker, Unity, HTML/Twine and more, on Windows.

**[Download the latest release →](https://github.com/AlbatrossLabs/VNDeck/releases/latest)**

| File | Use it if |
| --- | --- |
| `VN.Deck-Setup-x.y.z.exe` | You want it installed. It updates itself when a new version is out. |
| `VN.Deck-Portable-x.y.z.exe` | You want one file you can run from anywhere. It tells you about new versions; you download them yourself. |

VN Deck isn't code-signed yet, so Windows SmartScreen shows "unknown publisher" the first time. Choose **More info → Run anyway**.

**Requirements:** Windows 10 or 11, 64-bit. [7-Zip](https://7-zip.org) recommended for unpacking .rar files.

## Getting started

1. Run VN Deck and add the folder (or folders, on any drive) where your games live.
2. It scans them, groups versions of the same game, and pulls covers from the game files. Folders named "Completed", "On hold" and the like set each game's status.
3. Open **Review** to confirm which VNDB / itch.io / F95zone page belongs to each game. From then on VN Deck checks them for new versions.
4. Optional: add your itch.io API key in **Settings → Downloads & installs** so itch updates download and install by themselves.

## What it does

- **Finds your games.** Engine detection, version grouping, covers, play time per game and per version.
- **Knows when there's an update.** Looks each game up on VNDB, itch.io and F95zone with no account needed and checks for new versions on a schedule. Windows notifications and a tray badge when something's new.
- **Downloads and installs.** itch.io updates come through itch's official API. F95zone links open in VN Deck's own browser window: you click through the host's page, VN Deck catches the file and unpacks it next to the old version. Archives already sitting in your folders install in one click. Old versions can go to the Recycle Bin after their saves are backed up.
- **Ren'Py extras.** Controls profiles for keyboard, controller and arcade stick, applied at launch and removed after. Reading progress, a gallery unlock switch, and mods added for one session.
- **Saves.** Finds Ren'Py saves in AppData and game folders, backs them up, restores them, and searches them.
- **Organizes.** Tags (including tags imported from VNDB / itch / F95), smart views, filters, bulk edit, wishlist, hidden games, notes with checklists, art browser.
- **Couch mode.** Full screen for a TV, an arcade cabinet or a virtual screen in VR, driven by a controller, keyboard or arcade stick. Games launch full screen.
- **Privacy.** NSFW tag with blurred covers, discreet mode, optional app PIN.

### Couch mode controls

| Controller | Keyboard | Does |
| --- | --- | --- |
| D-pad / left stick | Arrow keys | Move |
| A | Enter | Open the game |
| B | Esc | Back (on a shelf: jump to its start) |
| X | X | Play right away |
| Y | F | Favorite |
| LB / RB | Q / E or Page Up / Page Down | Skip six games along a shelf |
| Start | M | Menu (leave couch mode, quit VN Deck) |
| Hold **RB**, press **Start** (in a game) | — | Quit the game, back to VN Deck |

Arcade sticks in keyboard mode (X-Arcade and similar) work out of the box. The in-game quit combo works in Ren'Py and HTML games; turn it off in **Settings → Couch mode**.

## Good to know

- **Your game folders are left alone.** VN Deck only reads them, with three exceptions: a temporary script it adds to Ren'Py games while they run (removed when they close), new versions you choose to install (always into a new folder), and old versions you choose to send to the Recycle Bin.
- **Unpacking** uses 7-Zip if it's installed, otherwise Windows' built-in `tar` (fine for .zip and .7z; .rar only on recent Windows 11).
- **F95zone:** VN Deck reads public pages and the latest-updates list politely, at most one request every 3 seconds. It never automates sign-in, masked links, countdowns or captchas. Downloads from F95 links always go through a page you click yourself.
- **Your data stays on your PC** in `%APPDATA%\VNDeck`. VN Deck sends nothing about you or your library anywhere; the only requests it makes are game-page lookups, downloads you start, and the update check.
- **Moving to a new PC:** **Settings → Backup & export** makes one .zip of your library (play time, notes, tags, covers, save backups) that you restore on the other PC.

## Feedback

Found a bug or have an idea? [Open an issue](https://github.com/AlbatrossLabs/VNDeck/issues). **Settings → About & updates → Logs** has a log you can copy into it.
