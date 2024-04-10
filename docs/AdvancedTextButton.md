# AdvancedTextButton
This is a AdvancedTextLabel that behaves like a button

Extends **AdvancedTextLabel**

![](assets/advanced-text-button-inspector.png)

## Table of Contents

- [**Vars**](#vars)
	- [**disabled**](#disabled)
	- [**toggle_mode**](#toggle_mode)
	- [**button_pressed**](#button_pressed)
	- [**button_group**](#button_group)
- [**Signals**](#signals)
	- [**pressed**](#pressed)
	- [**toggled**](#toggled)

## Vars

### disabled

*default value* : `false:`
If true, button will be disabled

### toggle_mode

*default value* : `false`
If true, button will be in toggle mode

### button_pressed

*default value* : `false:`
If true, button will be in pressed state

### button_group

*default value* : `""`
Name of node group to be used as button group
It changes all toggleable buttons in group in to radio buttons

## Signals

### pressed
Emitted when button is pressed

### toggled
 - (value)

Emitted when button is toggled
Works only if `toggle_mode` is on.
