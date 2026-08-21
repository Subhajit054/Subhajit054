# GitHub Profile v3 — Setup

1. Open https://github.com/Subhajit054
2. Open your profile repository (`Subhajit054`).
3. Replace its README.md with the README.md from this package.
4. Upload the entire `assets/` folder.
5. Commit the changes.

## Important
The hero is now a repository-local animated GIF:
`assets/evolution.gif`

The other visuals are repository-local SVGs:
- `assets/skills.svg`
- `assets/projects.svg`
- `assets/engineering.svg`
- `assets/telemetry.svg`

This means the main visuals do not depend on external image-hosting services.

The social buttons use Shields.io only for small badge graphics. The main profile visuals are local.

If you later want GitHub statistics, add a GitHub Actions workflow that writes generated SVG statistics into this repository. The current README deliberately uses a local telemetry panel instead of external stats images so you do not get broken-image icons.
