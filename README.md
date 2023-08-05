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

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/preview_dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/preview_light.png">
    <img alt="Preview image of the theme" src="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/preview_dark.png">
</picture>

## Customization

Various theme-related settings defined by Sublime Text, as well as a few custom settings specific to this theme are supported to tweak the appearance.
All settings should be modified in the *Preferences.sublime-settings* file, which can be opened via *Preferences > Settings* from the menu.

__Custom settings:__

| Setting | Default | Description |
| ------- | ------- | ----------- |
| "kind_icons_style" | "octicons" | Controls the style for the kind icons which are shown in the autocompletion popup and the "Goto Symbol" panels. Options:<ul><li>"octicons" (from GitHub)</li><li>"gitlab" (from GitLab)</li><li>"codicons" (from VS Code)</li><li>"letters" (similar to the built-in themes)</li></ul> |
| "git_status_icons" | "octicons" | Controls the style for the git status icons for files and folders in the sidebar. Options:<ul><li>"octicons"</li><li>"codicons"</li><li>"disabled"</li> |
| "sidebar_status_colors" | false | Highlight filenames in the sidebar for files with Git status "new" or "modified" in green and orange. Regardless of this setting, files with status "ignored" are always dimmed. |
| "popup_style" | "rounded" | Controls the style for hover popups. Options are "plain", "rounded" and "square". When set to "rounded" or "square", popups will be drawn with a border. |
| "tooltip_style" | "dark" | Controls the style for tooltips. Options are "dark" and "light". |
| "scroll_bar_style" | "auto" | Controls the style for scroll bars. Options are "brackets", "sublime", "thin" and "auto". The "auto" option uses "sublime" when overlay scroll bars are enabled, and "brackets" when disabled. |
| "fold_buttons_style" | "triangle" | Controls the style for the buttons shown in the gutter to fold regions of text. Options are "triangle" and "square". |
| "hide_tabs_dropdown_button" | false | Hides the tabs dropdown button. |
| "blend_inactive_tabs" | false | Blend the color of inactive tabs with the background. This is how inactive tabs in the built-in Default and Adaptive themes are shown. This setting only applies if "file_tab_style" is "rounded" or "square". |

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/kind_icons_dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/kind_icons_light.png">
    <img alt="Preview image of different kind icons styles" src="https://raw.githubusercontent.com/jwortmann/brackets-theme/master/img/kind_icons_dark.png">
</picture>

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

## File Icons

This theme uses custom file type icons in the sidebar.
As a side effect, file icons might not be displayed correctly when you switch to another theme, like for example the built-in *Default* or *Adaptive* themes.
To restore the icons for those themes, disable this package by running *Package Control: Disable Package* from the command palette and select *Theme - Brackets*.

## Attributions

* Git status icons in the sidebar and kind icons used in the autocompletion popup and the *Goto Symbol…* panels are derived from [Octicons](https://github.com/primer/octicons) (licensed under the [MIT license](/licenses/Octicons/LICENSE)), [GitLab SVGs](https://gitlab.com/gitlab-org/gitlab-svgs) (licensed under the [MIT license](/licenses/GitLabSVGs/LICENSE)) and [Codicons](https://github.com/microsoft/vscode-codicons) (licensed under [CC BY 4.0](/licenses/Codicons/LICENSE)).

* File icons in the sidebar are derived from [FileIcons](https://github.com/braver/FileIcons) (licensed under the [MIT license](/licenses/FileIcons/LICENSE)), [AFileIcon](https://github.com/SublimeText/AFileIcon) (licensed under the [MIT license](/licenses/AFileIcon/LICENSE.md)), [Material Icon Theme](https://github.com/PKief/vscode-material-icon-theme) (licensed under the [MIT license](/licenses/MaterialIconTheme/LICENSE.md)) and [Simple Icons](https://github.com/simple-icons/simple-icons) (licensed under CC0).

* Textures for the "wave" tab style are derived from [Theme - DAneo](https://github.com/SublimeText/Theme-DAneo) (licensed under the [MIT license](/licenses/DAneo/LICENSE)).
