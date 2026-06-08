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

Before publishing, replace the placeholder `publisher` value in `package.json` with your Marketplace publisher id.

Then publish with:

```bash
npm run publish:vsce
```