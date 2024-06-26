# RenPyMarkupParser

![img](assets/ren-inspector.png)

This parser is every limited as its just translates RenPy Markup to BBCode
This parser also adds Headers `{h1}`, `:emojis:` and icons `{icon:name}` add Rakugo variables with `<var_name>`

Extends **[ExtendedBBCodeParser]**

!!! See also

    [**RenPyMarkup**](Renpy.md)

## Funcs

### parse

- text: String

Returns given RenPyMarkup parsed into BBCode

### parse_links

- text: String

parse Ren'Py links into BBCode
Ren'Py links examples:

```
{a=https://some_domain.com}link{/a}
{a}https://some_domain.com{/a}
```

### parse_imgs

- text: String

parse Ren'Py images with out size into BBCode
Ren'Py images example:
`{img=<path>}`

### parse_imgs_size

- text: String

parse Ren'Py images with size into BBCode
Ren'Py images with size example:
`{img=<path> size=<height>x<width>}`

[ExtendedBBCodeParser]: ExtendedBBCodeParser.md
