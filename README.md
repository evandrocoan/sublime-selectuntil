# SelectUntil

Fill a void in your Sublime Text multiple selection capabilities! This plugin allows you to extend each selection until the next instance of a search term, making it super easy to edit multiple pieces of text that are similar but not quite the same enough.

## Usage

- <kbd>ctrl/alt</kbd> + <kbd>shift</kbd> + <kbd>s</kbd>: pulls up an input field, where you can type:

	- `search term` or `[search term]`: for each selection, select up to and including the first occurrence of the search term.
	- `/regex search/`: select through the first occurrence of the regex.
	- `{character count}`: select forward the given number of characters.
	- `-[search term]`: select backwards up to and including the search term.
	- `-/regex/`: backwards regex.
	- `-{character count}`: select backwards a certain number of characters (`{-count}` works too).

- <kbd>ctrl/alt</kbd> + <kbd>shift</kbd> + <kbd>s</kbd> a second time: reverses the search direction.

- <kbd>ctrl/alt</kbd> + <kbd>shift</kbd> + <kbd>r</kbd>: reverse all selections (so if the insertion point is at the end of the selection, it is moved to the beginning, and vice versa).

On Windows and Linux the default shortcuts use <kbd>alt</kbd>.  On OSX <kbd>ctrl</kbd> is used.


## Installation

### By Package Control

1. Download & Install **`Sublime Text 3`** (https://www.sublimetext.com/3)
1. Go to the menu **`Tools -> Install Package Control`**, then,
   wait few seconds until the installation finishes up
1. Go to the menu **`Tools -> Command Palette...
   (Ctrl+Shift+P)`**
1. Type **`Preferences:
   Package Control Settings – User`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
   add the following setting to your **`Package Control.sublime-settings`** file, if it is not already there
   ```js
   [
       ...
       "channels":
       [
           "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
           "https://packagecontrol.io/channel_v3.json",
       ],
       ...
   ]
   ```
   * Note,
     the **`https://raw...`** line must to be added before the **`https://packagecontrol...`**,
     otherwise you will not install this forked version of the package,
     but the original available on the Package Control default channel **`https://packagecontrol...`**
1. Now,
   go to the menu **`Preferences -> Package Control`**
1. Type **`Install Package`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
search for **`SelectUntil`** and press <kbd>Enter</kbd>

See also:
1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## Getting SelectUntil

The easiest way to get SelectUntil is with [Sublime Package Control](http://wbond.net/sublime_packages/package_control/installation).  Search for "SelectUntil".

Alternatively you can clone this git repository into your [Packages Directory](http://sublimetext.info/docs/en/basic_concepts.html):

	git://github.com/xavi-/sublime-selectuntil.git

## Developed by

* Xavi Ramirez
* [Nikolaus Wittenstein](https://github.com/adzenith)

## License

This project is released under [The MIT License](http://www.opensource.org/licenses/mit-license.php).
