# Card frame templates

Drop Magic Set Editor (MSE) style folders here. Each subfolder is one **frameset** the Card Creator can use.

## Folder layout

```
public/card-frames/
  magic-old.mse-style/
    wcard.jpg
    ucard.jpg
    bcard.jpg
    rcard.jpg
    gcard.jpg
    acard.jpg          # artifact (optional)
    ccard.jpg          # colorless (optional)
    mcard.jpg          # multicolor / gold (optional)
    xcard.jpg          # eldrazi colorless (optional)
    wlcard.jpg         # land variants (optional)
    ...
    frameset.json      # optional display name
```

## Color file names

| Code | Spell frame | Land frame |
|------|-------------|------------|
| W | `wcard.jpg` | `wlcard.jpg` |
| U | `ucard.jpg` | `ulcard.jpg` |
| B | `bcard.jpg` | `blcard.jpg` |
| R | `rcard.jpg` | `rlcard.jpg` |
| G | `gcard.jpg` | `glcard.jpg` |
| Artifact | `acard.jpg` | — |
| Colorless | `ccard.jpg` | `clcard.jpg` |
| Multicolor | `mcard.jpg` | `mlcard.jpg` |

PNG extensions are also supported (`.png` instead of `.jpg`).

## Optional `frameset.json`

```json
{
  "name": "Before 8th edition",
  "layout": "old-standard"
}
```

If omitted, the folder name (without `.mse-style`) is used as the display name.

## v1 supported layouts

Only **standard vertical** frames (375×523) with `*card.jpg` files. Split, saga, planeswalker, and clear/mask templates are not supported yet.

After adding or removing folders, restart the dev server (`npm run dev`).

Source: [Full-Magic-Pack](https://github.com/MagicSetEditorPacks/Full-Magic-Pack)
