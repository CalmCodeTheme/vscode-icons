# CalmCode Icons for VS Code

Это расширение добавляет набор SVG-икон для проводника VS Code. В проект уже скопированы все файлы из папки `calmcodeicons-zed/icons`, и они подключены через тему `CalmCode Icons`.

## Структура проекта

- `icons/` — все SVG-файлы иконок
- `themes/calmcodeicons.json` — маппинг иконок для VS Code
- `package.json` — манифест расширения

## Как запустить и проверить

1. Установите зависимости:
   ```bash
   npm install
   ```

2. Откройте папку проекта в VS Code.

3. Нажмите `F5` для запуска нового окна Extension Development Host.

4. В новом окне откройте Explorer и выберите тему иконок:
   - Command Palette → "Preferences: File Icon Theme"
   - выберите `CalmCode Icons`

5. Проверьте, что файлы и папки отображаются нужными SVG-иконками.

## Как сделать иконки активными в продакшн

1. Откройте `package.json` и замените:
   - `publisher`: на ваш ник в Marketplace
   - `repository.url`: на ваш GitHub репозиторий
2. Убедитесь, что в `icons/` лежат все SVG-файлы, и они корректно связаны через `themes/calmcodeicons.json`.
3. Запустите упаковку:
   ```bash
   npx @vscode/vsce package
   ```
   Это создаст файл `.vsix`.

## Как опубликовать в Marketplace

1. Зарегистрируйтесь в Azure DevOps / Visual Studio Marketplace и получите Personal Access Token (PAT).
2. Войдите в `vsce`:
   ```bash
   npx @vscode/vsce login your-name
   ```
3. Опубликуйте расширение:
   ```bash
   npx @vscode/vsce publish
   ```

Или напрямую:

```bash
npx @vscode/vsce package
npx @vscode/vsce publish
```

## Полезные ссылки

- VS Code Extension Manifest: https://code.visualstudio.com/api/references/extension-manifest
- VS Code File Icon Theme: https://code.visualstudio.com/api/extension-guides/file-icon-theme
- Publishing extensions: https://code.visualstudio.com/api/working-with-extensions/publishing-extension

## Дальнейшие улучшения

- добавить отдельные иконки для папок `src`, `components`, `public`, `test`
- сделать более аккуратную цветовую палитру для светлой и тёмной темы
- добавить custom icons для специфичные файлы вашего проекта
