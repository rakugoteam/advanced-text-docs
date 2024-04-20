# ExtendedBBCodeParser

![](assets/bb-inspector.png)

This parser adds Headers `{h1}`, `:emojis:` and icons `[icon:name]`
add Rakugo variables with `<var_name>` to BBCode

Extends **[TextParser](TextParser.md)**

!!! See also

    [**ExtendedBBCode**](ExtendedBBCode.md)

## Vars

### headers

_default value_ : `_gen_headers([22, 20, 18, 16])`

_Setting for headers_

By default those settings are just sizes: `22`, `20`, `18` and `16`.
Due to BBCode limitations `shadow_color` is used as background color.
Ignored properties: `line_spacing `, `shadow_offset `and `shadow_size`

## Funcs

### parse

- text: String

Generates LabelSettings set based on the given sizes
It is used to generate headers initial settings.
Must be run at start of parsing.
Needed for plugins with other addons to work
Returns given ExtendedBBCode parsed into BBCode

### parse_headers

- text: String

Parse headers in given text into BBCode

### parse_spaces

- text: String

Parse `[space=x]`, that it add space in text in size of x

### add_header

- header_size: int
- text: String
- add_new_line := false

Returns given text with added BBCode for header with given size (1-4) to it.
