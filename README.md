# DarkLight Hybrid Theme

A VS Code theme with a dark workbench and a light editor.

## Features

- Dark shell for the activity bar, side bar, panel, and status bar
- Light editor surface for comfortable code reading
- High-contrast syntax colors tuned for readability

## Get Started

1. Install dependencies:

   ```bash
   npm install
   ```

2. Open the workspace in VS Code and run the extension with the `Run Extension` debug configuration.

3. Open the Color Theme picker and choose `DarkLight Hybrid`.

## Package

Create a VSIX package with:

```bash
npm run package
```

## Publish

Then publish with:

```bash
npm run publish:vsce
```

## Auto Publish On GitHub Release

This repository is configured to publish automatically when a GitHub Release is published.

Workflow file:

- `.github/workflows/publish-on-release.yml`

What it does:

1. Runs on `release.published`.
2. Ensures release tag matches `package.json` version (`vX.Y.Z` tag format is supported).
3. Packages the extension as `darklight-hybrid-theme.vsix`.
4. Publishes to VS Code Marketplace using `VSCE_PAT`.
5. Uploads the VSIX to the GitHub release assets.

Required repository secret:

- `VSCE_PAT`: Personal Access Token from your VS Code Marketplace publisher account.

Release checklist:

1. Bump `version` in `package.json`.
2. Commit and push.
3. Create a GitHub release tag (for example `v0.0.2`) that matches the package version.