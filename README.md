# Brackets Theme for Sublime Text

[![License](https://img.shields.io/github/license/jwortmann/brackets-theme)](https://github.com/jwortmann/brackets-theme/blob/master/LICENSE)

A theme for Sublime Text inspired by Adobe Brackets.

This package only controlls the look of the UI in Sublime Text.
For the according syntax highlighting schemes also see my [Brackets Color Scheme](https://github.com/jwortmann/brackets-color-scheme), which can be installed separately.

## Installation

The package requires Sublime Text build 4107 or newer.
At this time, it can be manually installed by copying all files from this repository into a folder named *Theme - Brackets* under the *Packages* directory (*Preferences > Browse Packages* from the menu).

## Preview

![Preview dark](/img/preview_dark.png)

![Preview light](/img/preview_light.png)

## Customization

Various default theme-related settings defined by Sublime Text, as well as a few custom settings specific to this theme are supported to configure the appearance.
All settings should be modified in the *Preferences.sublime-settings* file.

| Setting | Default | Description |
| ------- | ------- | ----------- |
| "kind_letters" | `false` | Use the default style with colored kind letters instead of icons in autocompletion popups and the *Goto Symbol…* panel. |
| "sidebar_status_colors" | `false` | Highlight filenames in the sidebar for files with Git status "new" or "modified" in green and orange. Files with status "ignored" are always dimmed. |
| "hide_sidebar_status_icons" | `false` | Hide the Git status icons in the sidebar. |

## Attributions

* Kind icons used in the autocompletion popup and the *Goto Symbol…* panel, as well as icons indicating the Git status for sidebar entries are adapted from Microsoft's [Codicons](https://github.com/microsoft/vscode-codicons) icon font (licensed under [CC BY 4.0](/licenses/Codicons/LICENSE)).

* File icons in the sidebar are derived from [braver/FileIcons](https://github.com/braver/FileIcons) (licensed under the [MIT license](/licenses/FileIcons/LICENSE)).
