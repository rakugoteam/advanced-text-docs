# ExtendedBBCodeParser


Extends **TextParser**


## Vars
 - [**headers**](#headers)

## Funcs
 - [**parse**](#parse)
 - [**parse_headers**](#parse_headers)
 - [**parse_spaces**](#parse_spaces)
 - [**add_header**](#add_header)

## Vars
### headers
*default value* : `_gen_headers([22, 20, 18, 16])`

This parser adds Headers {h1}, :emojis: and icons [icon:name]

add Rakugo variables with <var_name> to BBCode

Setting for headers

By default those settings are just sizes: 22, 20, 18 and 16

Due to BBCode limitations shadow_color is used as background color

Ignored properties: line_spacing, shadow_offset and shadow_size


## Funcs
### parsetext:String
 - text:String

Generates LabelSettings set based on the given sizes

It is used to generate headers initial settings.

Must be run at start of parsing

Needed for plugins with other addons to work

Must be run at end of parsing

Needed for plugins with other addons to work

Returns given ExtendedBBCode parsed into BBCode

### parse_headerstext:String
 - text:String

Parse headers in given text into BBCode

### parse_spacestext:String
 - text:String

Parse [space=x], that it add space in text in size of x

### add_headerheader_size:int, text:String
 - header_size:int

 -  text:String

Returns given text with added BBCode for header with given size (1-4) to it

