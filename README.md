# Brackets Theme for Sublime Text

[![License](https://img.shields.io/github/license/jwortmann/brackets-theme)](https://github.com/jwortmann/brackets-theme/blob/master/LICENSE)
[![Version](https://img.shields.io/github/v/release/jwortmann/brackets-theme?label=version)](https://github.com/jwortmann/brackets-theme/releases)

A theme for Sublime Text inspired by Adobe Brackets.

This package only controlls the look of the user interface in Sublime Text.
For the according syntax highlighting schemes also see my [Brackets Color Scheme](https://github.com/jwortmann/brackets-color-scheme), which can be installed independently.

## Installation

The theme requires Sublime Text build 4107 or newer.
It can be installed with Sublime Text's package manager [Package Control](https://packagecontrol.io/installation).
From the command palette select *Package Control: Install Package* and search for *Theme - Brackets*.

## Preview

![Preview Dark](img/preview_dark.png)

![Preview Light](img/preview_light.png)

## Customization

Various theme-related settings defined by Sublime Text, as well as a few custom settings specific to this theme are supported to tweak the appearance.
All settings should be modified in the *Preferences.sublime-settings* file, which can be opened via *Preferences > Settings* from the menu.

__Custom settings:__

| Setting | Default | Description |
| ------- | ------- | ----------- |
| "kind_icons_style" | "octicons" | Controls the style for the kind icons which are shown in the autocompletion popup and the "Goto Symbol" panels. Options:<ul><li>"octicons" (from GitHub)</li><li>"codicons" (from VS Code)</li><li>"letters" (similar to the built-in themes)</li></ul> |
| "git_status_icons" | "octicons" | Controls the style for the git status icons for files and folders in the sidebar. Options:<ul><li>"octicons"</li><li>"codicons"</li><li>"disabled"</li> |
| "sidebar_status_colors" | false | Highlight filenames in the sidebar for files with Git status "new" or "modified" in green and orange. Regardless of this setting, files with status "ignored" are always dimmed. |
| "popup_style" | "default" | Controls the style for hover popups. Options are "default", "rounded" and "square". When set to "rounded" or "square", popups will be drawn with a border. |
| "tooltip_style" | "dark" | Controls the style for tooltips. Options are "dark" and "light". |
| "blend_inactive_tabs" | false | Blend the color of inactive tabs with the background. This is how inactive tabs in the built-in Default and Adaptive themes are shown. This setting only applies if "file_tab_style" is "rounded" or "square". |

__Relevant standard settings:__

| Setting | Default | Description |
| ------- | ------- | ----------- |
| "themed_title_bar" | true | Controls if a custom or default title bar is used. |
| "file_tab_style" | "rounded" | Controls the style of file tabs. Options: "rounded", "square", "angled", "wave". |
| "inactive_sheet_dimming" | true | If inactive sheets should have their background slightly modified to make input focus more obvious. |
| "highlight_modified_tabs" | false | Makes tabs with modified files more visible. |
| "overlay_scroll_bars" | "system" | Valid values are "system", "enabled" and "disabled". |
| "hide_tab_scrolling_buttons" | false | Hides the buttons for scrolling tabs left/right, requiring use of a trackpad or mouse scroll wheel. |
| "hide_new_tab_button" | false | Hides the new tab button. |
| "popup_shadows" | true | Draw shadows under popup windows. |

## Attributions

* Kind icons used in the autocompletion popup and the *Goto Symbol…* panels are derived from [Octicons](https://github.com/primer/octicons) (licensed under the [MIT license](/licenses/Octicons/LICENSE)) and from [Codicons](https://github.com/microsoft/vscode-codicons) (licensed under [CC BY 4.0](/licenses/Codicons/LICENSE)).

* Git status icons in the sidebar are derived from Octicons and from Codicons.

* File icons in the sidebar are derived from [FileIcons](https://github.com/braver/FileIcons) (licensed under the [MIT license](/licenses/FileIcons/LICENSE)).

* Textures for the "wave" tab style are derived from [Theme - DAneo](https://github.com/SublimeText/Theme-DAneo) (licensed under the [MIT license](/licenses/DAneo/LICENSE)).
