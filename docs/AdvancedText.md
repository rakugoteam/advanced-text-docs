# AdvancedText Singleton

This is singleton is used to keep references and common variables
for AdvancedText in one place and not duplicate them.
Mainly used to simplify the handling of supported addons/plugins.

Extends **Node**

## Vars

### root

This is singleton is used to keep references and common variables
for AdvancedText in one place and not duplicate them.
Mainly used to simplify the handling of supported addons/plugins.
Reference to root. Its a getter that returns `get_node("/root/").`

### rakugo

Reference to Rakugo singleton.
Its a getter that returns Rakugo singelton if it exist.

### emojis

Reference to EmojisDB singleton.
Its a getter that returns EmojisDB singelton if it exist.

### icons

Reference to IconsDB singleton.
Its a getter that returns MaterialIconsDB singelton if it exist.

## Funcs

### get_singleton

- singleton: String

Func used get singletons from other addons.
Build-in Engine.get_singleton() works only for C++ custom modules,
So we need to make this workaround.
