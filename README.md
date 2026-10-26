# Project Nostalgia Assets

Era-true Fortnite content images (mode tiles, backgrounds, news art) for every season's client.

## Structure
```
tiles/
  c3s1/   <- Chapter 3 Season 1 (v19.10) mode tiles + key art (83 files)
  c1s1/   <- (add per-season folders as they're built out)
  ...
backgrounds/  <- lobby backgrounds per season
news/         <- news tile art
```

## Usage
The backend's `contentpages_eras/era_sections.json` references these via:
```
https://raw.githubusercontent.com/ThunderboltnGamer/ProjectNostalgia-Assets/main/tiles/c3s1/<file>
```
The client downloads them directly (no auth needed - public repo).

## Sourced from
Epic's historical CDN (cdn2.unrealengine.com) - the original era files.

## Known missing (dead on Epic's CDN, not archived - drop replacements in if found)
- `19br-702x1024-0b760b5e9ac7.jpg` (the C3S1 Battle Royale vertical tile)
- `stw-702x1024-redesign-702x1024-ce3b6cf011f0.jpg` (the STW vertical)
- `creative-redesign-702x1024-d291d48aef3d.jpg` (the Creative vertical)
- 10 old LTM tiles (Blitz, SoloShowdown, FoodFight, 5x20, SolidGold, etc.)

These fall back to clean colored tiles / era substitutes in the content pages.
