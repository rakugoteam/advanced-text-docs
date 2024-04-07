# TextParser
Base class used by AdvancedTexts addon Parsers

Extends **Resource**

## Table of Contents

- [**Vars**](#vars)
	- [**re**](#re)
	- [**result**](#result)
	- [**replacement**](#replacement)
	- [**root**](#root)
- [**Funcs**](#funcs)
	- [**parse**](#parse)
	- [**get_singleton**](#get_singleton)
	- [**replace_regex_match**](#replace_regex_match)
	- [**to_bbcode_img**](#to_bbcode_img)
	- [**to_bbcode_link**](#to_bbcode_link)
	- [**safe_replace**](#safe_replace)

## Vars

### re

*default value* : `RegEx.new()`
RegEx used by this class

### result

Used to store result of last RegEx search

### replacement

*default value* : `""`
Used to store replacement for RegEx search

### root

Root ref is needed to check if other compatible addons are installed

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
 -  result: RegExMatch
 -  replacement: String

Func that my parsers uses to replace result in given text with replacement.

### to_bbcode_img
 - path: String
 -  size:=""

Returns given path to image as BBCode img
Size must be given as "<height>x<width>" without "< >"
Size is this way to be easy to use by Parsers

### to_bbcode_link
 - path: String
 -  link_text:=""

Returns given path/url to image as BBCode link
If link_text != "" it will be displayed as link text

### safe_replace
 - what: String
 -  for_what: String
 -  text: String

Used to replace given `what` Regex String
with `for_what` String in given text,
skipping parts of text that are in code tags,
for this to work `in_code = find_all_in_code(text)`
must be called first.
