# Shades of Purple — Theme Suite

A multi-app theme suite built on [**Shades of Purple**][upstream] by [Ahmad Awais][awais].
The original VS Code theme is the source of truth; this repo ports it across editors, terminals, and other apps, and adds a light variant for each target.

## What's inside

```
themes/
├── vscode/        # VS Code extension (source of truth)
├── warp/          # Warp terminal themes
└── openchamber/   # OpenChamber themes
```

| App | Variants | Source |
| --- | --- | --- |
| VS Code | Dark, Super Dark, Light, Italic | `themes/vscode/*.json` |
| Warp | Dark, Super Dark, Light | `themes/warp/*.yaml` |
| OpenChamber | Dark, Super Dark, Light | `themes/openchamber/*.json` |

The VS Code JSON theme files are the canonical source. The Warp and OpenChamber exports are derived from them — sync the VS Code files from upstream first, then regenerate the ports to match.

## Variants added beyond upstream

- **Light** — a light variant, not part of the upstream VS Code theme. Created for light/dark switchers.

Super Dark is part of the upstream VS Code theme (created by Ahmad Awais). This suite ports it to Warp and OpenChamber alongside the Dark and Light variants.

## Installation

### Warp

Copy the desired `themes/warp/shades-of-purple-*-warp.yaml` file into Warp's themes directory and reload themes in Warp settings:

- macOS: `~/.warp/themes/`

```sh
cp themes/warp/*.yaml ~/.warp/themes/
```

### OpenChamber

Copy the desired `themes/openchamber/*.json` file into OpenChamber's themes directory, then **Settings → Theme → Reload themes**:

- macOS/Linux: `~/.config/openchamber/themes/`

```sh
mkdir -p ~/.config/openchamber/themes
cp themes/openchamber/*.json ~/.config/openchamber/themes/
```

Then pick **Shades of Purple**, **(Light)**, or **(Super Dark)** from the dropdown.

### VS Code (from source)

The flagship theme is published by Ahmad Awais on the [VS Code marketplace][marketplace]. To use this suite's additions from source:

```sh
git clone https://github.com/thoom/shades-of-purple-themes.git \
  ~/.vscode/extensions/shades-of-purple-themes
```

Reload VS Code and select the theme from **Preferences → Color Theme**.

## Color palette

The palette is hand-picked for contrast and readability across all three variants. Colors are extracted from the VS Code theme JSON files.

| Usage | Dark | Super Dark | Light |
| --- | --- | --- | --- |
| Background | ![#2D2B55](https://img.shields.io/badge/-%232D2B55-2D2B55?style=flat-square) | ![#191830](https://img.shields.io/badge/-%23191830-191830?style=flat-square) | ![#FFFFFF](https://img.shields.io/badge/-%23FFFFFF-FFFFFF?style=flat-square) |
| Background Dark | ![#1E1E3F](https://img.shields.io/badge/-%231E1E3F-1E1E3F?style=flat-square) | ![#15152B](https://img.shields.io/badge/-%2315152B-15152B?style=flat-square) | ![#F2F0FF](https://img.shields.io/badge/-%23F2F0FF-F2F0FF?style=flat-square) |
| Foreground | ![#A599E9](https://img.shields.io/badge/-%23A599E9-A599E9?style=flat-square) | ![#A599E9](https://img.shields.io/badge/-%23A599E9-A599E9?style=flat-square) | ![#191830](https://img.shields.io/badge/-%23191830-191830?style=flat-square) |
| Hover Background | ![#4D21FC](https://img.shields.io/badge/-%234D21FC-4D21FC?style=flat-square) | ![#4D21FC](https://img.shields.io/badge/-%234D21FC-4D21FC?style=flat-square) | ![#E5E0FF](https://img.shields.io/badge/-%23E5E0FF-E5E0FF?style=flat-square) |
| Contrast | ![#FAD000](https://img.shields.io/badge/-%23FAD000-FAD000?style=flat-square) | ![#FAD000](https://img.shields.io/badge/-%23FAD000-FAD000?style=flat-square) | ![#FAD000](https://img.shields.io/badge/-%23FAD000-FAD000?style=flat-square) |
| Contrast Lite | ![#FFEE80](https://img.shields.io/badge/-%23FFEE80-FFEE80?style=flat-square) | ![#FFEE80](https://img.shields.io/badge/-%23FFEE80-FFEE80?style=flat-square) | ![#827717](https://img.shields.io/badge/-%23827717-827717?style=flat-square) |
| Contrast Lite II | ![#FAEFA5](https://img.shields.io/badge/-%23FAEFA5-FAEFA5?style=flat-square) | ![#FAEFA5](https://img.shields.io/badge/-%23FAEFA5-FAEFA5?style=flat-square) | ![#A48400](https://img.shields.io/badge/-%23A48400-A48400?style=flat-square) |
| Highlight | ![#FF7200](https://img.shields.io/badge/-%23FF7200-FF7200?style=flat-square) | ![#FF7200](https://img.shields.io/badge/-%23FF7200-FF7200?style=flat-square) | ![#E65100](https://img.shields.io/badge/-%23E65100-E65100?style=flat-square) |
| Comment | ![#B362FF](https://img.shields.io/badge/-%23B362FF-B362FF?style=flat-square) | ![#B362FF](https://img.shields.io/badge/-%23B362FF-B362FF?style=flat-square) | ![#8A4FD1](https://img.shields.io/badge/-%238A4FD1-8A4FD1?style=flat-square) |
| Constants | ![#FF628C](https://img.shields.io/badge/-%23FF628C-FF628C?style=flat-square) | ![#FF628C](https://img.shields.io/badge/-%23FF628C-FF628C?style=flat-square) | ![#D81B60](https://img.shields.io/badge/-%23D81B60-D81B60?style=flat-square) |
| Keywords | ![#FF9D00](https://img.shields.io/badge/-%23FF9D00-FF9D00?style=flat-square) | ![#FF9D00](https://img.shields.io/badge/-%23FF9D00-FF9D00?style=flat-square) | ![#BF7600](https://img.shields.io/badge/-%23BF7600-BF7600?style=flat-square) |
| Other (Meta) | ![#9EFFFF](https://img.shields.io/badge/-%239EFFFF-9EFFFF?style=flat-square) | ![#9EFFFF](https://img.shields.io/badge/-%239EFFFF-9EFFFF?style=flat-square) | ![#007399](https://img.shields.io/badge/-%23007399-007399?style=flat-square) |
| Strings | ![#A5FF90](https://img.shields.io/badge/-%23A5FF90-A5FF90?style=flat-square) | ![#A5FF90](https://img.shields.io/badge/-%23A5FF90-A5FF90?style=flat-square) | ![#1B5E20](https://img.shields.io/badge/-%231B5E20-1B5E20?style=flat-square) |
| Templates | ![#3AD900](https://img.shields.io/badge/-%233AD900-3AD900?style=flat-square) | ![#3AD900](https://img.shields.io/badge/-%233AD900-3AD900?style=flat-square) | ![#114014](https://img.shields.io/badge/-%23114014-114014?style=flat-square) |
| Definitions | ![#FB94FF](https://img.shields.io/badge/-%23FB94FF-FB94FF?style=flat-square) | ![#FB94FF](https://img.shields.io/badge/-%23FB94FF-FB94FF?style=flat-square) | ![#7B1FA2](https://img.shields.io/badge/-%237B1FA2-7B1FA2?style=flat-square) |
| Invalid | ![#EC3A37](https://img.shields.io/badge/-%23EC3A37-EC3A37?style=flat-square) | ![#EC3A37](https://img.shields.io/badge/-%23EC3A37-EC3A37?style=flat-square) | ![#EC3A37](https://img.shields.io/badge/-%23EC3A37-EC3A37?style=flat-square) |
| Diff Added | ![#35AD68](https://img.shields.io/badge/-%2335AD68-35AD68?style=flat-square) | ![#35AD68](https://img.shields.io/badge/-%2335AD68-35AD68?style=flat-square) | ![#2E7D32](https://img.shields.io/badge/-%232E7D32-2E7D32?style=flat-square) |
| Diff Removed | ![#EC3A37](https://img.shields.io/badge/-%23EC3A37-EC3A37?style=flat-square) | ![#EC3A37](https://img.shields.io/badge/-%23EC3A37-EC3A37?style=flat-square) | ![#C62828](https://img.shields.io/badge/-%23C62828-C62828?style=flat-square) |

## Acknowledgments

- **[Ahmad Awais][awais]** — creator of the original [Shades of Purple][upstream] VS Code theme and its hand-picked palette. All credit for the core colors and flagship dark theme belongs to him. This project is a downstream extension of his work.
- [OpenChamber][openchamber] — custom theme [format documentation][oc-themes].
- [Warp][warp] — terminal theme format.

## License

MIT — same as the original Shades of Purple theme. The upstream theme is Copyright © [Ahmad Awais](https://AhmadAwais.com/). Suite additions (the Light variant, plus the Warp and OpenChamber ports of all three variants) are released under the same MIT license.

[upstream]: https://github.com/ahmadawais/shades-of-purple-vscode
[marketplace]: https://marketplace.visualstudio.com/items?itemName=ahmadawais.shades-of-purple
[awais]: https://github.com/ahmadawais
[warp]: https://www.warp.dev
[openchamber]: https://github.com/openchamber/openchamber
[oc-themes]: https://github.com/openchamber/openchamber/blob/main/docs/CUSTOM_THEMES.md