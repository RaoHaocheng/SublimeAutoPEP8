### Sublime Auto PEP8 Formatting

## About
Automatically formats Python code to conform to the PEP 8 style guide using [autopep8](https://github.com/hhatto/autopep8) module
Supported ST3 only.

## Features
+ format / preview code according PEP8
+ format / preview selected text
+ format / preview all python modules in folder
+ side bar menu
+ formated code while saving

## Installing
The easiest way to install AutoPEP8 in through Package Control, which can be found at this site: [http://wbond.net/sublime_packages/package_control](http://wbond.net/sublime_packages/package_control)

Once you install Package Control, restart ST2/ST3 and bring up the Command Palette (`Command+Shift+P` on OS X, `Control+Shift+P` on Linux/Windows). Select "Package Control: Install Package", wait while Package Control fetches the latest package list, then select AutoPEP8 when the list appears.

## Settings
```javascript
{
    "settings": {
        "max-line-length": 79,

        // list codes for fixes; used by --ignore and --select
        "list-fixes": "",

        // do not fix these errors / warnings(e.g. E4, W)
        "ignore": "",

        // select errors / warnings(e.g. E4, W)
        "select": "",

        // number of spaces per indent level
        "indent-size": 4,

        "ignore-local-config": false,
        "global-config": "",

        "format_on_save": false,
        "show_output_panel": true,
        // Format/Preview menu items only appear for views
        // with syntax from `syntax_list`
        // value is base filename of the .tmLanguage syntax files
        "syntax_list": ["Python"],

        "file_menu_search_depth": 3, // max depth to search python files

        "avoid_new_line_in_select_mode": false,

        // print debug info into the console
        "debug": false,
        "logfile": "/tmp/sublimeautopep8.log"
    }
}
```

## Using

+ **SideBar** - right click on the file(s) or folder(s)
+ **Active view** - right click on the view
+ **Selected text** - right click on the selected text
+ **On Save** - provide by settings: option `format_on_save`
+ **Command Palette** - bring up the Command Palette and select `PEP8: Format Code` or `PEP8: Preview Changes`
+ **Hotkeys** - `Command/Control + Shift + 8` to format code, `Command/Control + 8` to preview changes
