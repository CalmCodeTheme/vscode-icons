# CalmCode Icons

Minimal, clean, and expressive SVG icon theme for VS Code.

CalmCode Icons gives your Explorer a calmer, more polished look with a soft palette, sharp readability, and support for a large set of popular languages, frameworks, config files, media assets, and common project folders.

## Supported file types

CalmCode Icons includes dedicated icons for the following file extensions and names:

### Programming languages and frameworks

- `.rs` — Rust
- `.js`, `.jsx` — JavaScript / React
- `.ts`, `.tsx` — TypeScript / React
- `.py` — Python
- `.go` — Go
- `.rb` — Ruby
- `.php` — PHP
- `.java` — Java
- `.kt`, `.kts` — Kotlin
- `.swift` — Swift
- `.dart` — Dart
- `.ex`, `.exs` — Elixir
- `.html`, `.htm` — HTML
- `.css`, `.scss`, `.sass`, `.less` — CSS / style files
- `.vue` — Vue
- `.svelte` — Svelte
- `.sql` — SQL / database files
- `.xml` — XML
- `.yaml`, `.yml` — YAML config
- `.toml` — TOML config
- `.json` — JSON
- `.svg` — SVG
- `.png`, `.jpg`, `.jpeg`, `.gif`, `.webp`, `.ico` — images
- `.mp4`, `.mp3`, `.wav` — media
- `.fbx`, `.obj`, `.stl`, `.step`, `.stp`, `.gltf`, `.glb` — 3D assets
- `.blend` — Blender
- `.tscn` — Godot scene files
- `.gd` — Godot scripts
- `.wgsl` — WGSL
- `.asm` — assembly
- `.ttf`, `.otf` — fonts
- `.txt` — plain text
- `.props` — property files
- `.class` — class files
- `.lock` — lock files
- `.svg` — vector graphics
- `.log` — logs

### Backend, tools, and config files

- `Cargo.toml` — Cargo manifest
- `package.json` — Node package manifest
- `tsconfig.json` — TypeScript config
- `jsconfig.json` — JavaScript config
- `README.md`, `README` — documentation
- `LICENSE` — license file
- `.gitignore` — Git ignore
- `.env` — environment file
- `Dockerfile`, `docker-compose.yml`, `docker-compose.yaml` — Docker
- `Makefile` — Make
- `CMakeLists.txt` — CMake
- `webpack.config.js` — webpack
- `vite.config.ts` — Vite
- `next.config.js` — Next.js
- `tailwind.config.js` — Tailwind
- `pyproject.toml`, `requirements.txt`, `setup.py` — Python setup
- `.gitattributes` — Git attributes
- `Makefile` — build tooling
- `.env` — environment variables
- `*.lock` — dependency lock files

### Languages and ecosystems included

- C
- C++
- C#
- F#
- Go
- Rust
- Python
- Java
- JavaScript
- TypeScript
- Node.js
- React
- Vue
- Svelte
- PHP
- Ruby
- Swift
- Dart
- Flutter
- Elixir
- Erlang
- Haskell
- Clojure
- Lua
- R
- Julia
- OCaml
- Kotlin
- Shell
- PowerShell
- Docker
- SQL
- 3D / model assets
- Game dev / Godot / WGSL

## Supported folders

CalmCode Icons also includes custom icons for common project folders and Git-related folders:

- `src`
- `.git`
- `node_modules`
- `test`
- `tests`
- `assets`
- `public`
- general project folders
- Git folders and open/closed folder states

## Theme behavior

The theme includes:

- file icons for common extensions
- file-name overrides for common manifests and config files
- folder icons for project structure patterns
- open/closed folder states
- special handling for git-related and source folders

## Install

1. Open VS Code
2. Go to Extensions
3. Search for `CalmCode Icons`
4. Click Install
5. Open the Command Palette and choose:
   - `Preferences: File Icon Theme`
   - select `CalmCode Icons`

## Development

This project is structured as follows:

- `icons/` — all SVG icon assets
- `themes/calmcodeicons.json` — VS Code theme mapping
- `package.json` — extension metadata and publishing config
- `assets/` — shared icon set used across editor integrations

## Local testing

```bash
npm install
```

Then launch the extension in a new development host:

1. Open the project in VS Code
2. Press `F5`
3. In the new window, pick `CalmCode Icons` as the active file icon theme

## Packaging

```bash
npx @vscode/vsce package
```

This generates a `.vsix` package for manual installation or Marketplace publication.

## Publish to Marketplace

```bash
npx @vscode/vsce login YOUR_PUBLISHER_NAME
npx @vscode/vsce publish
```

## Roadmap

- expand folder icon coverage
- refine the icon set for more project conventions
- add even more language-specific and tooling-specific icons
- improve consistency for both light and dark themes

## About

CalmCode Icons is built for developers who want a cleaner, calmer IDE without sacrificing clarity and discoverability.

The goal is simple: make your project tree easier to scan, easier to navigate, and more aesthetically consistent across the tools you use every day.
