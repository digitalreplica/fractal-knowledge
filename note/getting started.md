---
tags: a/note
---
in:: [[fractal knowledge]]

# Getting started
## Creating a knowledge set
### With a template


### Manually
Creating an empty knowledge set is simple, with only five files needed. Start by creating the index and topics.

> [!info] me/private/notes/index/index
> `---`
> `a/index`
> `---`
> `in:: [[topics]]`
> 
> `All knowledge starts with [[topics]]`

> [!info] me/private/notes/topic/topics
> `---`
> `a/topic`
> `---`
> `in:: [[index]]`

It is useful to create a default topic for notes

> [!info] me/private/notes/topics/general knowledge
> `---`
> `a/topic`
> `---`
> `in:: [[topics]]`

Create templates for notes and topics. 

> [!info] _templates/fractal-knowledge-core/a note template
> `---`
> `a/note`
> `---`
> `in:: [[general knowledge]]`

> [!info] _templates/fractal-knowledge-core/a topic template
> `---`
> `a/topic`
> `---`
> `in:: [[topics]]`

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
