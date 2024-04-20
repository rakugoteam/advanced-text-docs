# Emojis for Godot Support

!!! note

    First you need to have installed and enabled [Emojis for Godot addon](https://rakugoteam.github.io/addons/emojis-for-godot).

Emojs can be used with one of this nodes:

- [AdvancedTextLabel]
- [AdvancedTextButton]
- [AdvancedTextCheckButton]

!!! note

    See how to configure [AdvancedText Nodes].

![text-nodes][text-nodes]

Open **Icon Finder**, go to Godot's menu
_Project (1) > Tools (2) > Icon Finder (3)_
So you can find the icons easily.

![emoji-finder-menu-screenshot][emoji-finder-menu-screenshot]

You can search **(1)** emojis and change preview size **(2)**,
and click on emoji you want to use.

![emoji-finder-screenshot][emoji-finder-screenshot]

When you click on emoji you want to use it alias will be copy to system clipboard.

![emoji-finder-copy][emoji-finder-copy]

Now select Emoji node in scene tree.

![text-scene][text-scene]

Look at node **Inspector**, paste emoji alias using
(`Ctrl + V` or _Right Mouse Button > Paste_)
into `_text` as :emoji-name, size:

![text-inspector][text-inspector]

Now emojis are in your scene:

![addon-in-action][addon-in-action]

[AdvancedText Nodes]: HowToUse.md
[text-scene]: assets/text-scene.png
[addon-in-action]: assets/addon-in-action-emoji.png
[text-inspector]: assets/text-inspector-emoji.png
[text-nodes]: assets/text-nodes.png
[emoji-finder-copy]: assets/emoji-finder-copy.png
[emoji-finder-menu-screenshot]: assets/emoji-finder-menu.png
[emoji-finder-screenshot]: assets/emoji-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md
