# Mes Préférences Sublime Text 3

Tout d'abord il faut télécharger [Sublime Text 3](http://www.sublimetext.com/3) et le [package control](https://sublime.wbond.net/installation#st3).

## Cloner les préférences

Il faut tout d'abord se rendre dans le dossier `package` de sublime text :
```
cd ~/Library/Application\ Support/Sublime\ Text/Packages
```

Ensuite renomer l'ancien dossier `user` :

```
mv User User.old
``` 

Enfin, cloner le dépôt dans un nouveau dossier `user` :

```
git clone git@github.com:francoiscoron/Sublime-Text-Preference.git User
```

## Settings - User

Voici mes réglages par défaut pour l'interface de Sublime Text, la police `Source Code Pro` est disponible sur [google font](https://www.google.com/fonts) et le thème, Predawn, [ici](https://github.com/jamiewilson/predawn). Les lignes suivantes sont à ajouter dans `Sublime Text -> Preferences -> Settings -User` :

```json
{
    "caret_extra_width": 1,
    "caret_style": "phase",
    "close_windows_when_empty": false,
    "color_scheme": "Packages/Predawn/predawn.tmTheme",
    "copy_with_empty_selection": false,
    "drag_text": false,
    "draw_minimap_border": true,
    "enable_tab_scrolling": false,
    "folder_exclude_patterns":
    [
        ".svn",
        ".git",
        ".hg",
        "CVS",
        ".sass-cache",
        "tmp",
        "OLD",
        "Vendor",
        "node_modules"
    ],
    "font_face": "Source Code Pro",
    "font_options":
    [
        "no_round"
    ],
    "font_size": 15,
    "highlight_line": true,
    "ignored_packages":
    [
        "Vintage"
    ],
    "line_padding_bottom": 2,
    "line_padding_top": 2,
    "match_brackets_content": false,
    "match_selection": false,
    "match_tags": false,
    "open_files_in_new_window": false,
    "overlay_scroll_bars": "enabled",
    "preview_on_click": false,
    "scroll_speed": 5.0,
    "show_full_path": false,
    "tabs_medium": true,
    "theme": "predawn.sublime-theme",
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true,
    "word_wrap": true
}
```
Et mes préférences pour le `Markdown`, qui se trouve dans `Sublime Text -> Preference -> Settings - More -> Syntax Specific` :

```json
{
    "color_scheme": "Packages/Predawn/predawn-markdown.tmTheme",
    "draw_centered": true, // Centers the column in the window
    "draw_indent_guides": false,
    "font_size": 15,
    "trim_trailing_white_space_on_save": false,
    "word_wrap": true,
    "wrap_width": 60  // Sets the # of characters per line
}
```

