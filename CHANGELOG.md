Brackets Theme Changelog
========================

v1.12.0 (2025-09-14)
--------------------

  * Fixed opening wrong syntax specific settings file for filenames with special
    file icon.

  * Added various new file icons for the sidebar.

  * The "winui" theme variant now uses the color scheme's accent color to highlight
    matched characters in the command palette and in the auto-complete popup.


v1.11.0 (2025-05-24)
--------------------

  * Added support for the new "sidebar_on_right" setting.

  * Added a new file icon for Zsh.


v1.10.0 (2024-11-23)
--------------------

  * Added styling for checkboxes.

  * Fixed color for tab highlight indicator of new tabs.

  * Improvements and fixes for the "winui" theme variant.

  * Updated and added new file icons for the sidebar.

  * Removed the obsolete monochrome file icons for the sidebar.


v1.9.1 (2024-08-03)
-------------------

  * Updated styles for the "winui" theme variant.

  * Added new file icons for the sidebar.


v1.9.0 (2024-04-06)
-------------------

  * Replaced the monochrome gray file type icons in the sidebar with full colored icons.

  * New but unmodified tabs now have a green highlighting indicator, if the
    "highlight_modified_tabs" setting is enabled (only in ST build 4170 or newer).

  * Added a new "theme_variant" setting which can be set to "winui" in order to apply an
    alternative style for the title bar, the side bar, autocomplete popups, and other UI
    elements, inspired by the Windows 11 Mica & Acrylic materials.


v1.8.0 (2024-01-04)
-------------------

  * Redesigned the file tabs to make it more obvious which tab is currently selected.
    There is a new setting "tab_shadows" which can be set to false to revert back to the flat tab
    style that was used before.

  * Breaking change: The "blend_inactive_tabs" setting was renamed to "inactive_tab_transparency".
    It can be enabled if you prefer the style of inactive tabs from the Default and Adaptive themes.
    Now this setting also works if "file_tab_style" is set to "angled" or "wave".

  * Added and updated a few file icons in the sidebar.

  * Fixed popup border color with light color schemes if the "popup_style" setting is not used.

  * Removed support for previously deprecated setting names, which were still functional before
    this update.


v1.7.0 (2023-08-24)
-------------------

  * Added a new "gitlab" style option for the "kind_icons_style" setting.

  * Added a new "letters" style option for the "git_status_icons" setting.

  * Fixed padding and scroll bar color in the Switch Project window.

  * Fixed style for disabled button in the Update window.

  * Adjusted puck color of the "thin" scroll bar style to match the color from Windows Explorer.

  * Updated a few file type icons and added icon for Jupyter Notebook (.ipynb).

  * Updated and added new preview screenshots in the Readme page on GitHub.


v1.6.0 (2023-07-30)
-------------------

  * Updated sidebar design with a border on the left-hand side and additional margin at the top
    (only if the "themed_title_bar" setting is enabled).

  * The scroll bars in the sidebar now follow the "overlay_scroll_bars" setting - when disabled, the
    scroll bars are visible when hovering with the mouse over the sidebar.

  * Fixed a potential incompatibility with the LSP package for certain file types with special icons.


v1.5.0 (2023-07-20)
-------------------

  * Added a new setting "scroll_bar_style" with options "auto" (default), "brackets", "sublime" and
    "thin".

  * Minor style tweak for the default fold buttons.

  * Updated a few file type icons.


v1.4.0 (2023-06-21)
-------------------

  * Added a new setting "fold_buttons_style" with options "triangle" (default) and "square".

  * Added animations for fold buttons and for close buttons of modified tabs.

  * Updated and added a few new file type icons.


v1.3.1 (2023-06-10)
-------------------

  * Fixed included syntaxes for special file icons to be visible in file dialogs.


v1.3.0 (2023-06-09)
-------------------

  * Added new custom file type icons in the sidebar.

  * Hover popups are now rendered with a border and rounded corners by default. You can revert to
    the old style by adding "popup_style": "plain" into your settings.

  * Added the ability to hide the tabs dropdown button by using the setting
    "hide_tabs_dropdown_button": true.

  * Minor style tweak for selected and highlighted rows in the command palette (rounded corners).


v1.2.1 (2023-01-28)
-------------------

  * Fixed dash/minus sign not being rendered in tooltips.

  * Fixed kind icon alignment in some quick panel overlays provided by plugins.


v1.2.0 (2023-01-01)
-------------------

  * Changed the default kind icons in the autocomplete popup and "Goto Symbol..." panel. A new
    setting "kind_icons_style" was added and can be set to "codicons" to restore the former icons.

  * The "kind_letters" setting is deprecated - use "kind_icons_style": "letters" instead.

  * Removed the "kind_icon_ambiguous" setting and the ability to show an icon for this kind.

  * Changed the default git status icons in the sidebar. A new setting "git_status_icons" was added
    and can be set to "codicons" to restore the former icons.

  * The "hide_sidebar_status_icons" setting is deprecated - use "git_status_icons": "disabled"
    instead.

  * Tweaked the visual presentation of the command palette with a subtle border and an increased
    corner radius.

  * Tweaked the visual presentation of tooltips to match the style of the command palette. Tooltips
    now have a shadow and use a dark background by default.

  * Added a new "tooltip_style" setting with the options "dark" and "light".

  * Added a new "popup_style" setting with the options "default", "rounded" and "square".

  * Adjusted the default file icon in the sidebar for markup files (HTML, Markdown, etc.), so that
    it matches the style of the other file icons.

  * Fixed inactive sheet dimming not working for HtmlSheets.

  * Increased the inactive sheet dimming contrast for light color schemes.


v1.1.1 (2022-09-14)
-------------------

  * Fixed tab color not updating after temporary selecting tabs from the command palette input.

  * Fixed find results in the scroll bar being hidden under the puck position.

  * Tweaked label and close button alignment for selected tabs in the sidebar.


v1.1.0 (2021-11-28)
-------------------

  * Added a new setting "blend_inactive_tabs" to blend the color of inactive tabs with the
    background. This is how inactive tabs are shown in the built-in Default and Adaptive themes.
    This setting only applies if "file_tab_style" is "rounded" or "square".

  * Added red indicator in tabs for deleted files (when "highlight_modified_tabs" is enabled).

  * Added a new tab style: "wave".

  * Added settings schema for LSP-json.


v1.0.3 (2021-10-25)
-------------------

  * Added a setting whether to display the kind icon for the "ambiguous" kind in autocompletion
    popups. This kind is usually used for word-completions from the buffer, and its icon has been
    disabled by default now. To re-enable the icon, set `"kind_icon_ambiguous": true` in the
    Preferences.sublime-settings file. This setting doesn't apply, if the `"kind_letters"` setting
    is set to `true` (because there is no kind letter for the "ambiguous" kind).

  * Changed the Git status icon for modified files in the sidebar from a square to a circle.

  * Adjusted the background color for text input fields when a dark color scheme is used. This
    increases the contrast for placeholder texts, which previously were very difficult to read in
    most color schemes, because the font color cannot be controlled directly by a theme. The new
    background color is set to the color scheme's background now.

  * The font size in Widgets like the console panel and text input fields isn't fixed anymore and
    uses the global font size set by the user instead.


v1.0.2 (2021-08-08)
-------------------

  * Use custom close icon in annotations.

  * Changed font style for keybindings in the command palette to non-italic.


v1.0.1 (2021-07-25)
-------------------

  * Added indicator icon for files with unsaved changes in the Open Files section of the sidebar.

  * Fixed kind icons in autocomplete popup not working with small font sizes.

  * Fixed blurry tab scroll buttons if hardware acceleration is enabled.


v1.0.0 (2021-07-23)
-------------------

  * Initial release.
