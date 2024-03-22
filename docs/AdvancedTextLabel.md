# AdvancedTextLabel


Extends **RichTextLabel**


## Vars
 - [**parser**](#parser)

## Vars
### parser
This class parses given text to bbcode using given TextParser

By default links (staring from `http`) will be opened in web browser

For custom links you can connect to `custom_link` signal

Text to be parsed in too BBCode

Use it instead of `text` from RichTextLabel

I had to make this way as I can't override `text` var behavior

TextParser that will be used to parse `_text`

