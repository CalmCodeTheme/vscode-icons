# CalmCode Icons for VS Code

This extension adds a set of SVG icons for the VS Code Explorer. The project already includes all files from the `calmcodeicons-zed/icons` folder and connects them through the `CalmCode Icons` theme.

## Project structure

- `icons/` — all SVG icon files
- `themes/calmcodeicons.json` — icon mapping for VS Code
- `package.json` — extension manifest

## How to run and test

1. Install dependencies:
   ```bash
   npm install
   ```

2. Open the project folder in VS Code.

3. Press `F5` to launch a new Extension Development Host window.

4. In the new window, open Explorer and select the icon theme:
   - Command Palette → "Preferences: File Icon Theme"
   - choose `CalmCode Icons`

5. Check that files and folders are displayed with the appropriate SVG icons.

## How to activate the icons in production

1. Open `package.json` and replace:
   - `publisher`: with your Marketplace username
   - `repository.url`: with your GitHub repository
2. Make sure all SVG files are present in `icons/` and correctly linked via `themes/calmcodeicons.json`.
3. Package the extension:
   ```bash
   npx @vscode/vsce package
   ```
   This will create a `.vsix` file.

## How to publish to the Marketplace

1. Register in Azure DevOps / Visual Studio Marketplace and get a Personal Access Token (PAT).
2. Log in to `vsce`:
   ```bash
   npx @vscode/vsce login your-name
   ```
3. Publish the extension:
   ```bash
   npx @vscode/vsce publish
   ```

Or directly:

```bash
npx @vscode/vsce package
npx @vscode/vsce publish
```

## Useful links

- VS Code Extension Manifest: https://code.visualstudio.com/api/references/extension-manifest
- VS Code File Icon Theme: https://code.visualstudio.com/api/extension-guides/file-icon-theme
- Publishing extensions: https://code.visualstudio.com/api/working-with-extensions/publishing-extension

## Planned improvements

- add separate icons for folders such as `src`, `components`, `public`, and `test`
- create a cleaner color palette for both light and dark themes
- add custom icons for project-specific files
