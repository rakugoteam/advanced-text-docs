# Godot Material Icons Support

!!! note

    First you need to have installed and enabled [Godot Material Icons addon](https://rakugoteam.github.io/addons/material-icons).

Icons can be used with one of this nodes:

- [AdvancedTextLabel]
- [AdvancedTextButton]
- [AdvancedTextCheckButton]

!!! note

    See how to configure [AdvancedText Nodes].

![text-nodes]

Open **Icon Finder**, go to Godot's menu
_Project (1) > Tools (2) > Icon Finder (3)_
So you can find the icons easily.

![icon-finder-menu-screenshot]

You can search **(1)** icons and change preview size **(2)**,
and click on icon you want to use.

![icon-finder-screenshot]
When you click on icon you want to
use it alias will be copy to system clipboard.

![icon-finder-copy]

Now select Icon node in scene tree.

![text-scene]

Look at node **Inspector**, paste icon alias using
(`Ctrl + V` or _Right Mouse Button > Paste_)
into `_text` as `[icon:icon-name, size]`.

![text-inspector]
Now icons are in your scene:

![addon-in-action]

[AdvancedText Nodes]: HowToUse.md
[text-scene]: assets/text-scene.png
[addon-in-action]: assets/addon-in-action-icon.png
[text-inspector]: assets/text-inspector-icon.png
[text-nodes]: assets/text-nodes.png
[icon-scene]: assets/text-scene.png
[icon-finder-copy]: assets/icon-finder-copy.png
[icon-finder-menu-screenshot]: assets/icon-finder-menu.png
[icon-finder-screenshot]: assets/icon-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md
