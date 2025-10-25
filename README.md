# ubroker

## Installation

```
pip install -r requirements
```

## Internal dependencies (my other repos)

- `utils` (https://github.com/dfrankmv/utils)
- `binance` (https://github.com/dfrankmv/binance)

## Useful development resources

### VSCode setting: `python.analysis.extraPaths`

While the installation of my `utils` and `binance` packages works correctly at runtime, I'm encountering a linting issue where VS Code doesn't recognize the modules. As a workaround, I've had to include the installation directory in the settings.json file's python.analysis.extraPaths setting.

```python
"python.analysis.extraPaths": [
    "./.venv/src",
],
```

### VSCode extension: Add folders easily to workspace

This extension is extremely useful during development. It allows me to effortlessly add any folder to the current workspace simply by right-clicking. I found this feature particularly valuable because my dependencies, utils and binance, are installed in an editable format. Adding these specific dependency folders to the workspace enables VS Code to detect their respective Git repositories, allowing me to commit any changes to these libraries without having to leave my main development window. Specifically, I added `.venv/src/utils` and `.venv/src/binance` to my workspace.

```
Extension ID: hegedus-mark.add-folders-easily-to-a-workspace
```

### VSCode extension: Notion MarkDown

This extension is highly beneficial for editing Markdown files, significantly boosting productivity. If you're familiar with the slash (/) shortcuts in Notion, you'll find this tool an incredibly efficient and familiar way to insert elements.

```
Extension ID: UppariPavanKalyan.QuickMarkDown
```