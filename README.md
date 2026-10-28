# Cultivar

Cultivar is a variety of [JetBrains Mono](https://github.com/JetBrains/JetBrainsMono), a typeface made for developers, with some glyphs redrawn or swapped for alternates. See the [Changelog](Changelog.md) for what's different.

It is an unofficial project, not affiliated with or endorsed by JetBrains. It uses its own family name, so it installs alongside JetBrains Mono without conflicting.

## Installation

### Mac/Windows

1. [Download the latest release](https://github.com/dnlzro/cultivar/releases/latest).
2. Unzip the archive and install the font:
   - _Mac_. Select all font files in the folder and double-click them. Click the **Install Font** button.
   - _Windows_. Select all font files in the folder, right-click any of them, then pick **Install** from the menu.

### Linux

Open a terminal and run the following:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/dnlzro/cultivar/main/install_manual.sh)"
```

### Using it in your editor

Set the font family to `Cultivar`. For example, in Visual Studio Code:

1. Open `Preferences` → `Settings`, or press <kbd>Ctrl</kbd>+<kbd>,</kbd> (<kbd>Cmd</kbd>+<kbd>,</kbd> on Mac).
2. In **Editor: Font Family**, type `Cultivar`, replacing any content.
3. To enable ligatures, go to **Editor: Font Ligatures**, click **Edit in settings.json**, and add `"editor.fontLigatures": true`.

In JetBrains IDEs, go to `Settings` → `Editor` → `Font` and pick **Cultivar** from the **Font** dropdown.

## Building from source

The sources in the `sources` folder are [Glyphs](https://glyphsapp.com) files. To build the `.ttf`, `.otf`, `.woff2` and variable fonts you need Python 3.11 or later:

```bash
pip install -r requirements.txt
gftools builder sources/config.yaml
python scripts/generate_variable_webfonts.py
```

The built files are written to the `fonts` folder.

## Releases

Built fonts aren't committed to the repository. CI builds them, and pushing a tag that starts with `v` creates a draft GitHub Release with the fonts attached.

## License

Cultivar is available under the [OFL-1.1 License](OFL.txt), like JetBrains Mono. The source code is available under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).

## Credits

Cultivar is based on JetBrains Mono, designed by Philipp Nurullin with Konstantin Bulenkov as team lead, with thanks to Nikita Prokopov, Eugene Auduchinok, Tatiana Tulupenko, Dmitrij Batrak, the IntelliJ Platform UX Team and the JetBrains Web Team.
