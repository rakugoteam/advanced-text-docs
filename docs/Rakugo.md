# Rakugo Dialogue System Support

!!! note

    First you need to have installed and enabled[Godot RDS addon](https://rakugoteam.github.io/rakugo-dialogue-system).
    RDS addon works only in Runtime mode.

This allows to use RakuVars in side text.
RakuVars can be used with one of this nodes:

- [AdvancedTextLabel][AdvancedTextLabel]
- [AdvancedTextButton][AdvancedTextButton]
- [AdvancedTextCheckButton][AdvancedTextCheckButton]

!!! note

    See how to configure[AdvancedText Nodes][AdvancedText Nodes].

![text-nodes][text-nodes]

First you have to crate a [GDScript or RakuScript that defines some RakuVariables](https://rakugoteam.github.io/rakugo-docs/2.2/rkvars/).

![text-scene][text-scene]

Look at node **Inspector**, to text add whit choosen RakuVars in `<>`,
for example `<some_var>` , you can use RakuVars in text tags:

!!! note

    Current way RDS uses very raw way of converting RakuVars values to strings.
    Because of this to use color in text like in example below there is need to use workaround:
    ```GDScript
    raku.set_variable("test_color", "#" + Color(1, 0.5, 1))
    ```

![text-inspector][text-inspector]

Now RakuVars are in your scene:

![addon-in-action][addon-in-action]

[AdvancedText Nodes]: HowToUse.md
[text-scene]: assets/text-scene.png
[addon-in-action]: assets/addon-in-action-raku.png
[text-inspector]: assets/text-inspector-raku.png
[text-nodes]: assets/text-nodes.png
[emoji-finder-copy]: assets/emoji-finder-copy.png
[emoji-finder-menu-screenshot]: assets/emoji-finder-menu.png
[emoji-finder-screenshot]: assets/emoji-finder.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md
