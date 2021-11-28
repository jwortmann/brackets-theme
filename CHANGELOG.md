Brackets Theme Changelog
========================

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
