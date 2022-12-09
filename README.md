# AutoSaveExt VSCode Extension

> VSCode extension for advanced autosave feature configuration.

This extension allows to have custom configuration of autosave feature for specified types of files because standard editor's `autoSave` option is applied to all file types and languages.

## Settings

Extension loads config from standard settings (project's `.vscode/settings.json` or .global user settings). 

This option is not language specific, so just add file extensions that should be a subject for autosave.

Supported config:

```json5
{
  "autoSaveExt": {
    "debounce": 1000, // default is 500
    "extensions": [".elm", ".ts"] // if no extension set will be applied to all files
  }
}
```

## Issues

If you have proposal or issue. Add an issue with description of your case.

### Unreleased

Initial release of unreleased yet.

## TODO
Add another feature of safe delayed autosave:
* when this is enabled, changes are synced to filename.ext.bk
* when Cmd + S is clicked, sync the content from filename.ext.bk to filename.ext
* when vscode exits, delete all filename.ext.bk
