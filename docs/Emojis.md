# Emojis for Godot Support

!!! note

    Those works only in runtime and not in editor.

First you need to have installed and enabled Emojis for Godot addon:

1. Download: <https://rakugoteam.github.io/addons/emojis-for-godot>
2. Unzip to *res:\\addons* dir
3. Go to menu > *Project > Projects Settings > Plugins*
4. Enable *Godot Material Icons*

After that you can use icons in  one of this nodes:
- [AdvancedTextLabel]
- [AdvancedTextButton]
- [AdvancedTextCheckButton]

![text-nodes]

Open **Icon Finder**, go to Godot's menu
_Project (1) > Tools (2) > Icon Finder (3)_
So you can find the icons easily.

![emoji-finder-menu-screenshot]

You can search **(1)** emojis and change preview size **(2)**,
and click on emoji you want to use.

![emoji-finder-screenshot]

When you click on emoji you want to use it alias will be copy to system clipboard.

![emoji-finder-copy]

Now select Emoji node in scene tree.

![text-scene]

Look at node **Inspector**, paste emoji alias using
(`Ctrl + V` or *Right Mouse Button > Paste*)
into `_text` as :emoji-name, size:

![text-inspector]

Now emojis are in your scene:

![addon-in-action]

[addon-in-action]:assets/addon-in-action-emoji.png
[text-inspector]:assets/text-inspector-emoji.png
[text-nodes]:assets/icon-nodes.png
[emoji-scene]:assets/emoji-scene.png
[emoji-finder-copy]:assets/emoji-finder-copy.png
[emoji-finder-menu-screenshot]:assets/emoji-finder-menu.png
[emoji-finder-screenshot]:assets/emoji-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md