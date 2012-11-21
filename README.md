# Typographic hotkeys [closed]

_Project is about to close_. Look for <a href="">*Web-developer's keyboard*</a> – replacement of Typographic hotkeys. It will be built as native Windows application.

Reasons of escaping:

* It's difficult to implement nice GUI with Autohotkey. It only suggests simple basic components, which is not very suitable for application's cases. C/C++ will allow to make even Metro UI.
* Any crossplatform idea is hacked at the root; C/C++ code will allow to think about migration.
* Autohotkey swarms with bugs, which is difficult to catch and to understand.
* It's unusual syntax of autohotkey scripts (something between Pascal, JavaScript and Basic ‽) and a lot of oddities.
* Difficult debugging of DllCalls and memory-related tasks.


## Description

Typographic Hotkeys™ extends default Windows keyboard with cool typographic tools. Script enables <a href="http://www.nouilles.info/keyboard_shortcuts.html">Mac OS X special characters shortcuts</a>, <a href="http://help.ubuntu.com/community/GtkComposeTable">Linux compose keys</a> premised with <a href="http://docs.oracle.com/cd/E19683-01/806-4743/6jdq6q2n7/index.html">Solaris compose keys</a> and other combinations, easy input of <a href="http://www.w3schools.com/tags/ref_symbols.asp">HTML symbol codes</a>, <a href="http://ilyabirman.ru/projects/typography-layout/">Ilya Birman keyboard layout</a> behaviour, **MS Office**-like autocorrection and other typographic opportunities. Besides, Web Designer's Keyboard℠ supplies a _color convertor_, that can transform recognized colors in selection to target color format, _get utf code_ function, that can get utf code of selected symbol, _in-place fake data generator_.

## Installation
1. Download and install <a href="http://www.autohotkey.com/">Autohotkey</a>™
2. Download <a href="http://dmitry-ivanov.me/playground/windows_typographic_hotkeys/TypographicHotkeys.ahk">TypographicKeyboard.ahk</a>, put it anywhere (i. e. _My Documents_) and open it with Autohotkey™

## Use Cases

### Inserting characters

There are few ways to insert special characters.

1. **Shortcuts**. Use <a href="http://www.nouilles.info/keyboard_shortcuts.html">OS X shortcuts for special characters</a>, just as if you were using Mac. For example, <kbd>Alt</kbd> + <kbd>-</kbd> = `–`, <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>-</kbd> = `—`, … See <a href="">full list of shortcuts</a>.
2. **Compose Keys**. Symbols are inserted by means of typing some characters while <kbd>Compose Key</kbd> being pressed. <kbd>Compose Key</kbd> is assigned to the <kbd>AltGr</kbd> (the same as <kbd>Right Alt</kbd>). Compose combinations vastly extended to cover a lot more than just Linux/Solaris combinations, see <a href="">full list</a>.
3. **Typing in brackets**. Type sequence in square brackets, and it will be automatically changed to according symbol, if exists one. For example, `[beta]` will be changed to `β`, and `[mdash]`, as well as `[---]` will be changed to `—`. Supports <a href="http://www.w3schools.com/tags/ref_symbols.asp">HTML Symbol Codes</a>, compose key combinations and other sequences (see full list).
4. **Windows characters** method. You can still type keys by `Alt + uCode`. For example, `Alt+0151` will get `—`. Unicode sequences included to combinations, so typing `[0151]` will result the same.

### Autoreplacements

Sequences below will be automatically transformed when typing has finished

 * `(c)` → `©`
 * `(r)` → `®`
 * `...` → `…`

### [pending] Convert color

Transforms found colors in selected string to passed format. For exaple, select `, rgba(25,45,32,.43)`. Hold <kbd>Menu key</kbd>, type rgb and selection will be transformed to [TODO] `, rgb(?,?,?)`. Supported format conversions: rgb, rgba, hsl, hsla, hex, #, plain.
! Supposed that background is white (most common case). Do not use alpha conversion with background other than white.
Nice use case: select all your css, press <kbd>Menu Key + rgb</kbd>, all recognized colors will be converted to `rgb` format. It will enhance rendering of page %)

### [pending] Get code

Html, utf

### [pending] Fake data generator

Text, dif languages, fake data, fake imgs

## TODO:

* Fake address
* Color convertor
* typographic test pages (font, type elements)
* html elements ()
* all possible symbols from utfgraphics
* gethtmlcode, getutf
* readme
* numerous tests
* pr: habrahabr, typographic community, authors of blogs, questions in forums, official forum, mythgol, retrogroup vk, Alex Bur, Korolkova, UTF table idea, Serof Lexa, Wikipedia, get link on script in every comment with (c)…
* rename to the web-designer keyboard, make rgb convertor
* cyrillics full cover & combos & extended
* think & make scenarious: habr image, linux user become windows, etc 
* wikipedia typographic symbols
* a lot of documentation
* make .exe and test autoload (startup)
* fix all bugs
* Make text selected when lorem ipsum generator worked out. It will allow to copy or delete this text



## Have done
* Densed kbd shortcuts
* Lorem ipsum localisation
* <a href="http://ilyabirman.ru/projects/typography-layout/">Ilya Birman keyboard</a> behaviour
* Lorem Ipsum generator
* Windows <a href="http://en.wikipedia.org/wiki/Alt_code">Alt-codes</a> extended to UTF
* <a href="http://www.nouilles.info/keyboard_shortcuts.html">Mac OSX Shortcuts</a>
* Auto startup
* Linux & Solaris compose keys