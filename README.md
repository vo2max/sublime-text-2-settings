Sublime Text Settings
=====================

These are personal settings for ST2. Having not yet used ST3, I cannot vouch as to if these settings are transferable to the newer version or not. **Use at your own risk**.

Requirements
------------

- [Sublime Text 2](http://www.sublimetext.com/)
- [Package Control](https://sublime.wbond.net/installation#st2)
- [Node.js](http://nodejs.org) - Required for HTML Prettify

Installation
------------

#### <i class="icon-folder-open"></i> GIT (via command-line)

1. Navigate to the Sublime Text 2 Packages directory.
   ```
   cd /cygdrive/C/Users/[USER]/AppData/Roaming/Sublime\ Text\ 2/Packages/
   ```

2. Clone the repository's .git folder into a empty temporary directory.
   ```
   git clone https://github.com/vo2max/sublime-text-settings.git User/UserTmp
   ```

3. Move the .git folder to the `User` directory. This makes the `User` directory a git repo. Then, delete the temporary directory.
   ```
   mv User/UserTmp/.git User/
   rm -rf User/UserTmp
   rmdir User/UserTmp
   ```

4. Revert the state of the local repo to HEAD (git believes the local files are deleted). **This will overwrite any local changes.**
   ``` 
   cd User
   git reset --hard HEAD
   ```

#### <i class="icon-folder-open"></i> GIT (via TortoiseSVN)

1. In Explorer, navigate to:
   ```
   C:\Users\[USER]\AppData\Roaming\Sublime Text 2\Packages
   ```

2. Checkout the repository into the `User` directory.
   ```
   SVN Checkout... -> 
   Repo: https://github.com/vo2max/sublime-text-settings.git/trunk
   Checkout dir: C:\Users\[USER]\AppData\Roaming\Sublime Text 2\Packages\User\
   ```

3. Confirm prompt for export into a non-empty folder.


#### <i class="icon-download"></i> Required Packages

Read [<i class="icon-share"></i> Package Control](https://sublime.wbond.net/installation#st2) for details regarding installation (itself, as well as other packages).

Packages
--------

#### General Tools
- [Alignment](http://wbond.net/sublime_packages/alignment)
- [BracketHighlighter (go to closing tag) [disable quotes in user settings]](https://github.com/facelessuser/BracketHighlighter)
- [Case Conversion](https://github.com/jdc0589/CaseConversion)
- [ChangeQuotes](https://github.com/colinta/SublimeChangeQuotes)
- [ColorPicker](http://weslly.github.io/ColorPicker/)
- [DeleteBlankLines](https://github.com/NicholasBuse/sublime_DeleteBlankLines)
- [Emmet](https://github.com/sergeche/emmet-sublime)
- [Find++](https://github.com/twolfson/FindPlusPlus)
- [FreeMarker](https://github.com/briancavalier/textmate-freemarker-bundle)
- [Gist (Snipppet management)](https://github.com/condemil/Gist)
- [Open URL](https://github.com/noahcoad/open-url)
- [StringEncode (converts char from one "encoding" to another)](https://github.com/colinta/SublimeStringEncode)
- [Sublimerge Pro](http://www.sublimerge.com/)

#### File Transfer
- [SFTP](http://wbond.net/sublime_packages/sftp)

#### Version Control

#### Code Intelligence
- [Jedi - Python Autocompletion](https://github.com/srusskih/SublimeJEDI)
- [SublimeCodeIntel (HTML autocomplete)](https://github.com/SublimeCodeIntel/SublimeCodeIntel)
- [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter-for-ST2)

#### Project Management
- [Nettuts Fetch](https://github.com/weslly/Nettuts-Fetch)

#### HTML
- [HTML Snippets](https://github.com/joshnh/HTML-Snippets)
- [HTML-CSS-JS Prettify](https://github.com/victorporof/Sublime-HTMLPrettify)
- [HTMLAttributes (HTML attribute autocomplete)](https://github.com/agibsonsw/HTMLAttributes)

#### CSS
- [Bootstrap 3 Snippets](https://github.com/JasonMortonNZ/bs3-sublime-plugin)
- [CSS Snippets](https://github.com/joshnh/CSS-Snippets)
- [LESS](https://github.com/danro/LESS-sublime)
- [LESS-build](https://github.com/berfarah/LESS-build-sublime)

#### JavaScript
- [Javascript Beautify](https://github.com/enginespot/js-beautify-sublime)
- [PyV8](https://github.com/emmetio/pyv8-binaries)
- [Sublime-KnockoutJS-Snippets](https://github.com/aaronpowell/Sublime-KnockoutJS-Snippets)

#### Ruby 

#### PHP

#### Databases

#### Server Configs

#### TeX

#### Flash

#### Java

Key Bindings
------------

|Command|Shortcut (Win)|
| :-------- | --------:| :--: |
|Select opening/closing tag (BracketHighlighter) | alt+up/down|
|Move a line up/down | ctrl+shft+up/down|
|Delete a line | ctrl+shft+k|
|Select contents of an element (Tag) | ctrl+shft+a or alt+a|
|Select all instances | alt+f3|
|Select next occurance(s) | ctrl+d|
|To lowercase | ctrl+k+l|
|Auto-format tags on selection | ctrl+alt+f|
|Rename tag shortcut (single quote) | ctrl+alt+'|

References
----------

#### Packages

[Package Control](https://sublime.wbond.net)

#### SFTP

[Using Sublime Text 2 and SFTP to work on remote files](http://coderwall.com/p/52p2xa)

#### Shortcuts

[Keyboard Shortcuts - Windows/Linux](http://docs.sublimetext.info/en/latest/reference/keyboard_shortcuts_win.html)  
[Sublime Text 2 – Useful Shortcuts (PC)](https://gist.github.com/1736542)

#### SSHFS (SSH Filesystem)

[Dokan SSHFS 0.6.0 released](http://dokan-dev.net/en/2011/01/12/dokan-sshfs-0-6-0-released/)

#### Syncing

[Syncing: Using Git/Dropbox](https://sublime.wbond.net/docs/syncing)