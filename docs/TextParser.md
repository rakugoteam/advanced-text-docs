# TextParser


Extends **Resource**


## Vars
 - [**re**](#re)
 - [**result**](#result)
 - [**replacement**](#replacement)
 - [**in_code**](#in_code)

## Funcs
 - [**parse**](#parse)
 - [**replace_regex_match**](#replace_regex_match)
 - [**to_bbcode_img**](#to_bbcode_img)
 - [**to_bbcode_link**](#to_bbcode_link)
 - [**find_all_in_code**](#find_all_in_code)
 - [**is_in_code**](#is_in_code)
 - [**safe_replace**](#safe_replace)

## Vars
### re
*default value* : `RegEx.new()`

Base class used by AdvancedTexts addon Parsers

RegEx used by this class

### result
Used to store result of last RegEx search

### replacement
*default value* : `""`

Used to store replacement for RegEx search

### in_code
*default value* : `[]`

Here will be stored all code between code tags in given text


## Funcs
### parsetext:String
 - text:String

This only exits to be override by Parsers classes that inherits from it

This func just returns given with out any changes

### replace_regex_matchtext:String, result:RegExMatch, replacement:String
 - text:String

 -  result:RegExMatch

 -  replacement:String

Func that my parsers uses to replace result in given text with replacement.

### to_bbcode_imgpath:String, size := ""
 - path:String

 -  size := ""

Returns given path to image as BBCode img

Size must be given as "<height>x<width>" without "< >"

Size is this way to be easy to use by Parsers

### to_bbcode_linkpath:String, link_text := ""
 - path:String

 -  link_text := ""

Returns given path/url to image as BBCode link

If link_text != "" it will be displayed as link text

### find_all_in_codetext:String, open_code_tag:="[code]", close_code_tag:="[/code]"
 - text:String

 -  open_code_tag:="[code]"

 -  close_code_tag:="[/code]"

It find all code in between code tags in given text

And add its start and end paris into in_code array,

to make easy to skip them in parsing process

This func should be run as first in parse()

### is_in_coderesult:RegExMatch
 - result:RegExMatch

It checks if given result is in code tags

used to skip parts of text that are in code tags in parsing process

### safe_replacewhat:String, for_what:String, text:String
 - what:String

 -  for_what:String

 -  text:String

Used to replace given `what` Regex String

with `for_what` String in given text,

skipping parts of text that are in code tags,

for this to work `in_code = find_all_in_code(text)`

must be called first.

