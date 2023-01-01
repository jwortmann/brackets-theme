Brackets Theme Changelog
========================

v1.2.0 (2023-01-)
-------------------

  * Changed the default kind icons in the autocomplete popup and "Goto Symbol..." panel. A new
    setting "kind_icons_style" was added and can be set to "codicons" to restore the former icons.

  * The "kind_letters" setting is deprecated - use "kind_icons_style": "letters" instead.

  * Removed the "kind_icon_ambiguous" setting and the ability to show an icon for this kind.

  * Changed the default git status icons in the sidebar. A new setting "git_status_icons" was added
    and can be set to "codicons" to restore the former icons.

  * The "hide_sidebar_status_icons" setting is deprecated - use "git_status_icons": "disabled"
    instead.

  * Tweaked the visual presentation of the command palette with a subtle border and increased
    corner radius.

  * Tweaked the visual presentation of tooltips to match the style of the command palette. Tooltips
    have a shadow and use a dark background now.

  * Adjusted the default file icon in the sidebar for markup files (HTML, Markdown, etc.), so that
    it matches the style of the other file icons.


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
