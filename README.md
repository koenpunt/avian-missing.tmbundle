# Avian Missing

This is a collection of missing features from [TextMate 2.0 Alpha](http://blog.macromates.com/2011/textmate-2-0-alpha/).
This bundle includes:

## <kbd>⌃⌘S</kbd> Save Project

The save project command will now create a `.tm_properties` in the current file browser folder
precompiled with `projectDirectory` set and an example `windowTitle` featuring the
current scm-branch and the `$projectDirectory` basename

**Example:**
```
 application.rb     ☛master     [awesome-app]
```

This command also saves the project in the favorities (accessible with `⌘⇧O`).


## <kbd>⎋</kbd> Character class indifferent completion

TextMate 2 [introduced](http://blog.macromates.com/2012/clever-completion/) strict …err …clever completion, which will not cross boundaries between character classes anymore. For example in Ruby typing `au` and hitting `⎋` for autocompletion will not pick `:auto` or `@autocomplete` since they have a leading `:` and `@` and the belong to the *symbol* and *instance variable* character classes.

This bundle reintroduces the TM1 behavior.


## <kbd>⌃⎋</kbd> Cross tab completion

[RubyAMP](http://code.leadmediapartners.com/) used to have this.


## <kbd>⌃⌥⌘T</kbd> Open Project directory in Terminal

_NOTE: requires OSX Lion_

Opens the current project directory in the terminal (not really present in TM1, but useful anyway).


## <kbd>⌃⌥⌘L</kbd> Keep current file as reference

> …waiting for split panes

Outputs the current source into the bottom html pane, this makes the current file source visible while changing tabs.

Seems that most of the need for split panes is to keep one file as a reference, this solves this particular issue.


## <kbd>⌥⌘,</kbd> Open the global `.tm_properties` with
Tired of opening `.tm_properties` from the terminal or browsing to it by hand?

Now you can just hit `⌥⌘,` and bring up your alternative preferencies (from you the home folder).


## <kbd>⌘S</kbd> Strip trailing whitespace on save

Just add `TM_STRIP_WHITESPACE_ON_SAVE = true` to your `.tm_properties`.
Ending newline fix is included.


## <del><kbd>⌃⌘N</kbd> New File</del> → <kbd>⇧⌘N</kbd> (builtin)

Removed as <kbd>⇧⌘N</kbd> has been introduced as a builtin command.



<br><br>

## Installation

```bash
mkdir -p ~/Library/Application\ Support/Avian/Bundles
cd ~/Library/Application\ Support/Avian/Bundles
git clone git://github.com/elia/avian-missing.tmbundle.git
```


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request


## Copyright

Copyright © 2012 Elia Schito. See MIT-LICENSE for details.
