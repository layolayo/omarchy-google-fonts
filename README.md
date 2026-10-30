# omarchy-google-fonts

A lightweight standalone script to download, extract, and install the complete [Google Fonts](https://github.com/google/fonts) `.ttf` collection on [Omarchy](https://omarchy.org/) and Arch Linux systems.

Adapted from the classic Ubuntu script by Michalis Georgiou and Andrew (WebUpd8).

## Quick Install (One-Liner)

### User Installation (Recommended — No `sudo` required)
Installs all `.ttf` fonts into `~/.local/share/fonts/google-fonts` and refreshes the font cache:

```bash
curl -fsSL https://raw.githubusercontent.com/layolayo/omarchy-google-fonts/main/install-google-fonts | bash
```

### System-Wide Installation
Installs all `.ttf` fonts into `/usr/share/fonts/google-fonts`:

```bash
curl -fsSL https://raw.githubusercontent.com/layolayo/omarchy-google-fonts/main/install-google-fonts | bash -s -- --system
```

## Using with Omarchy

Once the script finishes, all Google monospace fonts are immediately available to Omarchy's font manager:

```bash
# List available monospace fonts
omarchy font list

# Switch your system monospace font
omarchy font set "Google Sans Code"
```
