# How To use

AdvancedText nodes:

- [AdvancedTextLabel][AdvancedTextLabel]
- [AdvancedTextButton][AdvancedTextButton]
- [AdvancedTextCheckButton][AdvancedTextCheckButton]

![text-nodes][text-nodes]

Add one to scene.

![text-scene][text-scene]

Look at node **Inspector**

![text-inspector][text-inspector]

1. **BBCode Enabled** must be `true` for node to work.
2. You must choose one of **[TextParsers]**:
   * Load or crate new one of:
     * **[BBCodeExtendedParser]**
     * **[RenPyMarkupParser]**
     * **[MarkdownParser]**
     * Custom one that extends a **[TextParser]**
3. Then you can start to typing text in **Text** (`_text` in code)

Example how your **AdvnacedTextLabel** can look in scene:

![addon-in-action][addon-in-action]

[text-scene]: assets/text-scene.png
[addon-in-action]: assets/addon-in-action.png
[text-inspector]: assets/advanced-text-inspector.png
[text-nodes]: assets/text-nodes.png
[AdvancedTextLabel]: AdvancedTextLabel.md
[AdvancedTextButton]: AdvancedTextButton.md
[AdvancedTextCheckButton]: AdvancedTextCheckButton.md
[ExtendedBBCodeParser]: ExtendedBBCodeParser.md
[RenPyMarkupParser]: RenPyMarkupParser.md
[MarkdownParser]: MarkdownParser.md
[TextParser]: TextParser.md