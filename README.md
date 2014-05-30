Sublime Text Settings	{#welcome}
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
   git clone --no-checkout https://github.com/vo2max/sublime-text-settings.git User/User.tmp
   ```

3. Move the .git folder to the `User` directory. This makes the `User` directory a git repo. Then, delete the temporary directory.
   ```
   mv User/User.tmp/.git User/
   rmdir User/User.tmp
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
   Checkout dir: (current directory)
   ```

3. Confirm prompt for export into a non-empty folder.


#### <i class="icon-download"></i> Required Packages

Read [<i class="icon-share"></i> Package Control](https://sublime.wbond.net/installation#st2) for details regarding installation (itself, as well as other packages).

Packages
--------

#### General Tools
- [Alignment](http://wbond.net/sublime_packages/alignment)
- BracketHighlighter (go to closing tag) [disable quotes in user settings]
- Case Conversion
- ChangeQuotes
- DeleteBlankLines
- Emmet
- Find++
- FreeMarker
- Gist (Snipppet management)
- Open URL
- StringEncode (converts char from one "encoding" to another)
- Sublimerge Pro
- Tag (auto-complete closing tag, select tag contents)
#### File Transfer
- SFTP
#### Version Control
#### Code Intelligence
- Jedi - Python Autocompletion
- SublimeCodeIntel (HTML autocomplete)
- SublimeLinter
#### Project Management
- Nettuts Fetch
#### HTML
- HTML Snippets
- HTML-CSS-JS Prettify
- HTMLAttributes (HTML attribute autocomplete)
#### CSS
- Bootstrap 3 Snippets
- CSS Snippets
- LESS
- LESS-build
#### JavaScript
- Javascript Beautify
- PyV8
- Sublime-KnockoutJS-Snippets
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
SFTP
:   [Using Sublime Text 2 and SFTP to work on remote files](http://coderwall.com/p/52p2xa)

Shortcuts
:   [Keyboard Shortcuts - Windows/Linux](http://docs.sublimetext.info/en/latest/reference/keyboard_shortcuts_win.html)
:   [Sublime Text 2 – Useful Shortcuts (PC)](https://gist.github.com/1736542)

SSHFS (SSH Filesystem)
:   [Dokan SSHFS 0.6.0 released](http://dokan-dev.net/en/2011/01/12/dokan-sshfs-0-6-0-released/)
