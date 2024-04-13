# Godot Material Icons Support

First you need to have installed and enabled Godot Material Icons addon:

1. Download: <https://rakugoteam.github.io/addons/material-icons>
2. Unzip to *res:\\addons* dir
3. Go to menu > *Project > Projects Settings > Plugins*
4. Enable *Godot Material Icons*

After that you can use icons in  one of this nodes:
- [AdvancedTextLabel]
- [AdvancedTextButton]
- [AdvancedTextCheckButton]

![icon-nodes]

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

![icon-scene]

Look at node **Inspector**, paste icon alias using
(`Ctrl + V` or *Right Mouse Button > Paste*)
in to `_text`

![icon-inspector]

Now icons are in your scene:

![addon-in-action]

[addon-in-action]:assets/addon-in-action.png
[icon-inspector]:assets/icon-inspector.png
[icon-scene]:assets/icon-scene.png
[icon-nodes]:assets/icon-nodes.png
[icon-finder-copy]:assets/icon-finder-copy.png
[icon-finder-menu-screenshot]:assets/icon-finder-menu.png
[icon-finder-screenshot]:assets/icon-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md