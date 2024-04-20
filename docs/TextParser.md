# TextParser

Base class used by AdvancedTexts addon Parsers

Extends **[Resource](https://docs.godotengine.org/en/4.2/classes/class_resource.html)**

## Vars

### re

_default value_ : `RegEx.new()`

RegEx used by this class

### result

Used to store result of last RegEx search

### replacement

_default value_ : `""`

Used to store replacement for RegEx search

## Funcs

### parse

- text: String

This only exits to be override by Parsers classes that inherits from it
This func just returns given with out any changes

### get_singleton

- singleton: String

Func used get singletons from other addons

### replace_regex_match

- text: String
- result: RegExMatch
- replacement: String

Func that my parsers uses to replace result in given text with replacement.

### to_bbcode_img

- path: String
- size: String

Returns given path to image as BBCode img
Size must be given as "`<height>`x `<width>`" without "< >"
Size is this way to be easy to use by Parsers

### to_bbcode_link

- path: String
- link_text: String

Returns given path/url to image as BBCode link
If `link_text != ""` it will be displayed as link text

### safe_replace

- what: String
- for_what: String
- text: String

Used to replace given `what` Regex String
with `for_what` String in given text,
must be called first.
