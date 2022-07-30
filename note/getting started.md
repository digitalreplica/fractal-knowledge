---
tags: a/note
---
in:: [[fractal knowledge]]

# Getting started
## Creating a knowledge set
### With a template
A template for starting a knowledge set is located at [digitalreplica/fractal-knowledge-core-template |  GitHub](https://github.com/digitalreplica/fractal-knowledge-core-template) with instructions on how to download it and open it as an [Obsidian vault](https://help.obsidian.md/User+interface/Vault+switcher#Create+new+vaults)

### Manually
Creating an empty knowledge set is simple, with only a few files needed. Start by creating a new Obsidian vault, and add these files.

**me/private/notes/index/index**
```
---
a/index
---
in:: [[topics]]

All knowledge starts with [[topics]]
```

**me/private/notes/topic/topics**
```
---
a/topic
---
in:: [[index]]

The default topic to link topics to.
```

**me/private/notes/topics/general knowledge**
```
---
a/topic
---
in:: [[topics]]

Create templates for notes and topics.
```

**_templates/fractal-knowledge-core/a note template**
```
---
a/note
---
in:: [[general knowledge]]
```

**_templates/fractal-knowledge-core/a topic template**
```
---
a/topic
---
in:: [[topics]]
```

# Configure Obsidian
Here are Obsidian configuration settings that work well with fractal knowledge

Enable plugins
- Templates

Configuration | Setting
--- | ---
Default location for new notes | `me/private/notes/note`
Excluded files | `_templates/`
Template folder location | `_templates`

## Obsidian plugins
 The [breadcrumbs](https://breadcrumbs-wiki.onrender.com/docs/Home) makes navigation extremely simple. Fractal knowledge works well with a customized [heirarchy](https://breadcrumbs-wiki.onrender.com/docs/Getting%20Started/Hierarchies).

Direction | Heirarchy
--- | ---
up | in, up
same | near, same
