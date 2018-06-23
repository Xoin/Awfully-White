# Awfully White
Themable light theme for the new Facepunch forums using Less.

## Development
### Visual Studio Code
Recommended extensions:
[Less IntelliSense](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-less) for autocompletion
[Easy LESS](https://marketplace.visualstudio.com/items?itemName=mrcrowl.easy-less) Auto-compile LESS to CSS on save
Quick setup:
```json
{
	"folders": [
		{
			"path": "Awfully-White",
		}
	],
	"settings": {
		"less.compile": {
			"compress": true, // true => remove surplus whitespace
			"sourceMap": true, // true => generate source maps (.css.map files)
			"out": "${workspaceRoot}\\",
			"main": "${workspaceRoot}\\Awfullywhite.less"
		},
		"less.lint.duplicateProperties": "warning",
		"less.lint.important": "warning",
		"less.scannerExclude": [
			"${workspaceRoot}\\**/.git",
			"**/node_modules",
			"**/bower_components"
		]
	}
}
```
