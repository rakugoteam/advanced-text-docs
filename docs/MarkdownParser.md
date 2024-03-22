# MarkdownParser


Extends **ExtendedBBCodeParser**


## Vars
 - [**italics**](#italics)
 - [**bold**](#bold)
 - [**points**](#points)

## Funcs
 - [**parse**](#parse)
 - [**parse_spaces**](#parse_spaces)
 - [**parse_headers**](#parse_headers)
 - [**parse_imgs**](#parse_imgs)
 - [**parse_imgs_size**](#parse_imgs_size)
 - [**parse_links**](#parse_links)
 - [**parse_hints**](#parse_hints)
 - [**parse_sing**](#parse_sing)
 - [**parse_italics**](#parse_italics)
 - [**parse_bold**](#parse_bold)
 - [**parse_strike_through**](#parse_strike_through)
 - [**parse_code**](#parse_code)
 - [**parse_table**](#parse_table)
 - [**parse_color_key**](#parse_color_key)
 - [**parse_color_hex**](#parse_color_hex)
 - [**parse_effect**](#parse_effect)
 - [**parse_keyword**](#parse_keyword)
 - [**parse_points**](#parse_points)
 - [**parse_number_points**](#parse_number_points)
 - [**parse_list**](#parse_list)

## Vars
### italics
*default value* : `"*"`

This parser is every limited as its just translates Markdown to BBCode

This parser also adds :emojis: and icons {icon:name} add Rakugo variables with <var_name>

choose to use * or _ to open/close italics tag

### bold
*default value* : `"**"`

choose to use * or _ to open/close bold tag

### points
*default value* : `"-"`

choose to use - or * to make points in bulleted list


## Funcs
### parsetext: String
 - text: String

returns given Markdown parsed into BBCode

### parse_spacestext: String
 - text: String

Parse @space=x, that it add space in text in size of x

### parse_headerstext: String
 - text: String

Parse md # Headers in given text into BBCode

### parse_imgstext: String
 - text: String

Parse md images to in given text to BBCode

Example of md image: ![](path/to/img)

### parse_imgs_sizetext: String
 - text: String

Parse md images with size to in given text to BBCode

Example of md image with size: ![height x width](path/to/img)

### parse_linkstext: String
 - text: String

Parse md links to in given text to BBCode

Examples of md link:

[link](path/to/file.md)

<https://www.example.com>

### parse_hintstext: String
 - text: String

Parse md hint to in given text to BBCode

@[text](hint)

### parse_singtext: String, open: String, close: String, tag: String
### parse_italicstext: String
 - text: String

Parse md italics to in given text to BBCode

Example of md italics:

If italics = "*" : *italics*

If italics = "_" : _italics_

### parse_boldtext: String
 - text: String

Parse md bold to in given text to BBCode

Example of md bold:

If bold = "**" : **bold**

If bold = "__" : __bold__

### parse_strike_throughtext: String
 - text: String

Parse md strike through to in given text to BBCode

Example of md strike through: ~~strike through~~

### parse_codetext: String
 - text: String

Parse md code to in given text to BBCode

Example of md code:

one line code: `code`

multiline code: ```code```

### parse_tabletext: String
 - text: String

Parse md table to in given text to BBCode

Example of md table:

@tabel=2 {

| cell1 | cell2 |

}

### parse_color_keytext: String
 - text: String

Parse md color name from Color class tag to in given text to BBCode

### parse_color_hextext: String
 - text: String

Parse md color hex to in given text to BBCode

### parse_effecttext: String, effect: String, args: Array
 - text: String

 -  effect: String

 -  args: Array

Parse md effects to in given text to BBCode

### parse_keywordtext: String, keyword: String, tag: String
 - text: String

 -  keyword: String

 -  tag: String

Parse md keyword to in given text to BBCode

### parse_pointstext: String
 - text: String

Parse md points list to in given text to BBCode

### parse_number_pointstext: String
 - text: String

Parse md number points list to in given text to BBCode

### parse_listtext: String, open: String, close: String, regex: String
 - text: String

 -  open: String

 -  close: String

 -  regex: String

Parse md list to in given text to BBCode

