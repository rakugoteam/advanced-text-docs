# Emojis For Godot Support

First you need to have installed and enabled Emojis For Godot addon:

1. Download: <https://rakugoteam.github.io/addons/material-icons>
2. Unzip to *res:\\addons* dir
3. Go to menu > *Project > Projects Settings > Plugins*
4. Enable *Emojis For Godot*

After that you can use emojis in  one of this nodes:
- [AdvancedTextLabel]
- [AdvancedTextButton]
- [AdvancedTextCheckButton]

![text-nodes]

Open **Emoji Finder**, go to Godot's menu
_Project (1) > Tools (2) > Emoji Finder (3)_
So you can find the emojis easily.

![emoji-finder-menu-screenshot]

You can search **(1)** emojis and change preview size **(2)**,
and click on emoji you want to use.

![emoji-finder-screenshot]

When you click on emoji you want to use it alias will be copy to system clipboard.

![emoji-finder-copy]

Now select Emoji node in scene tree.

![text-scene]

Look at node **Inspector**,
paste emoji alias using (`Ctrl + V` or *Right Mouse Button > Paste*)
into `_text` between `::` like this `:emoji-name:`,
you can also change it size, for example `:e-mail, 24:`

![text-inspector]

Now emojis are in your scene:

![addon-in-action]

[addon-in-action]:assets/addon-in-action.png
[emoji-finder-copy]:assets/emoji-finder-copy.png
[emoji-finder-menu-screenshot]:assets/emoji-finder-menu.png
[emoji-finder-screenshot]:assets/emoji-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md
[text-inspector]:assets/text-inspector.png
[text-scene]:assets/text-scene.png
[text-nodes]:assets/text-nodes.png