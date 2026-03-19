# Zimbabwe Theme Collection

<p align="center">
  <img src="./images/logo.png" alt="Zimbabwe Theme — shield inspired by the Zimbabwe flag" width="160" />
</p>

A VS Code theme collection built around places people recognize in Zimbabwe. Each location comes in a dark and light variant, giving teams eight polished options that feel local, memorable, and easy to work in for long coding sessions.

## Included Themes

### Victoria Falls
- **Dark**: Deep basalt, spray mist, river teal, and sunset gold.
- **Light**: Clean mist whites, soft aqua, and warm lookout highlights.

### Harare
- **Dark**: Jacaranda dusk, city night tones, and warm urban amber accents.
- **Light**: Airy lavender haze, garden greens, and a crisp metropolitan surface.

### Chitungwiza
- **Dark**: Terracotta streets, energetic market color, and bright turquoise contrast.
- **Light**: Sunlit clay, warm township tones, and fresh contemporary accents.

### Bulawayo
- **Dark**: Heritage stone, railway steel, muted acacia greens, and dry-season gold.
- **Light**: Sandstone neutrals, civic warmth, and measured historic elegance.

## Design Direction

These themes were reworked to feel more intentional and place-led, rather than just flag-colored. The palette treatment takes cues from premium themes like Dobri Next Bunker: richer editor surfaces, stronger contrast discipline, and accent colors used with restraint so the themes stay expressive without becoming noisy.

## Why Users Install It

- Clear dark and light options for every featured place.
- Distinct personalities across themes while keeping syntax readable.
- Zimbabwe-inspired palettes that feel specific, not generic.
- Suitable for daily development, demos, and personal workspace branding.

## Installation

### From a VSIX release
1. Download the latest `.vsix` file from the project releases.
2. Open VS Code.
3. Go to `Extensions`.
4. Open the extensions menu and choose `Install from VSIX...`.
5. Select the downloaded package.

### From the terminal

### VS Code

```bash
code --install-extension /zimbabwe-theme-0.3.0.vsix
```

### Cursor

Cursor installs VS Code–compatible extensions the same way. From a terminal (with the [Cursor shell command](https://docs.cursor.com/) on your `PATH`):

```bash
cursor --install-extension ./zimbabwe-theme-0.3.0.vsix
```

Or in the app: **Extensions** → **⋯** → **Install from VSIX…** → choose the downloaded file.

If `cursor` is not found, open the Command Palette in Cursor and run **Shell Command: Install `cursor` command in PATH** (wording may vary slightly by version), then try the command again.

## Activate a Theme

1. Open the Command Palette with `Cmd/Ctrl + Shift + P`.
2. Run `Preferences: Color Theme`.
3. Choose one of the Zimbabwe themes:
   - `Zimbabwe - Victoria Falls Dark`
   - `Zimbabwe - Victoria Falls Light`
   - `Zimbabwe - Harare Dark`
   - `Zimbabwe - Harare Light`
   - `Zimbabwe - Chitungwiza Dark`
   - `Zimbabwe - Chitungwiza Light`
   - `Zimbabwe - Bulawayo Dark`
   - `Zimbabwe - Bulawayo Light`

## For Clients and Teams

If you are packaging this for a client, the collection gives you a cleaner story to present: a locally rooted theme suite with clear naming, paired light and dark modes, and enough variety for different user tastes without fragmenting the product.

## Deployment

This repo can publish on deploy to both marketplaces:

- VS Code Marketplace via `npx @vscode/vsce publish`
- Open VSX via `npx ovsx publish`

To enable that in GitHub Actions, add these repository secrets:

- `VSCE_PAT`: Personal access token for the Visual Studio Marketplace publisher.
- `OVSX_PAT`: Personal access token for Open VSX.

The workflow at `.github/workflows/release.yml` will package the extension, create a GitHub release, then publish to each marketplace when the matching secret is present.
