# RenPyMarkupParser


Extends **ExtendedBBCodeParser**


## Funcs
 - [**parse**](#parse)
 - [**parse_links**](#parse_links)
 - [**parse_imgs**](#parse_imgs)
 - [**parse_imgs_size**](#parse_imgs_size)

## Funcs
### parsetext: String
 - text: String

This parser is every limited as its just translates RenPy Markup to BBCode

This parser also adds Headers {h1}, :emojis: and icons {icon:name} add Rakugo variables with <var_name>

Returns given RenPyMarkup parsed into BBCode

### parse_linkstext: String
 - text: String

parse Ren'Py links into BBCode

Ren'Py links examples:

{a=https://some_domain.com}link{/a}

{a}https://some_domain.com{/a}

### parse_imgstext: String
 - text: String

parse Ren'Py images with out size into BBCode

Ren'Py images example:

{img=<path>}

### parse_imgs_sizetext: String
 - text: String

parse Ren'Py images with size into BBCode

Ren'Py images with size example:

