# AdvancedTextButton

This is a AdvancedTextLabel that behaves like a button

Extends **[AdvancedTextLabel](AdvancedTextLabel.md)**

![](assets/advanced-text-button-inspector.png)

## Vars

### disabled

_default value_ : `false`

If true, button will be disabled

### toggle_mode

_default value_ : `false`

If true, button will be in toggle mode

### button_pressed

_default value_ : `false`

If true, button will be in pressed state

### button_group

_default value_ : `""`

Name of node group to be used as button group
It changes all toggleable buttons in group in to radio buttons

## Signals

### pressed

Emitted when button is pressed

### toggled

- value : `bool`

Emitted when button is toggled
Works only if `toggle_mode` is on.
