---
tags: a/note
---
in:: [[fractal knowledge]]

# Basic usage
## Navigation
### Index
The index is intended for you to link to your favorite notes and topics, so you can find them quickly.

### In field
The `in` field navigates up, from a note to a topic, from a topic to all topics.

### Quick switcher
The quick switcher is an easy way to move to well known notes like the index. It seems to include folder names when searching, so `fr get` finds the fractal knowledge `getting started` page.

## Backlinks
Backlinks are the primary navigation method. From the [[topics]] page, you can find backlinks to all topics. From each topic, you can find backlinks to notes in that topic, and subtopics if it has them.

## Tags
All notes are tagged with `a` and the type of note. So topics can be found with `a/topic`, and so on.

## Breadcrumbs
The breadcrumbs plugin provides two great way to navigate. The matrix view is a little cleaner than backlinks for jumping quickly from all topics to a topic to a note. The trail view goes the other way, from a note, through all topics. Codeblocks are also nice, to embed downlinks into the topics page.

## Taking notes
### A simple note
The `general knowledge` topic is intended for quick notes about anything. It's the default topic for new notes. A note might look like

> [!info] me/private/notes/note/my note
> `---`
> `a/note`
> `---`
> `in:: [[general knowledge]]`
> 
> I have a note!

### Notes around a new topic

The simplest example is a single topic with a single note.

> [!info] me/private/notes/topic/cooking
> `---`
> `a/topic`
> `---`
> `in:: [[topics]]`

> [!info] me/private/notes/note/my cooking note
> `---`
> `a/note`
> `---`
> `in:: [[cooking]]`
> 
> I have a cooking note!

### Creating a shared repository
- Have one topic `in [[topics]]` so it'll show up on other's topics list.
- Make other topics as needed that point to your topic.
- Create notes pointing to your topics.
- Create a `repository` note, with at least the url to your knowledge repository.

## Shared knowledge example
### Recipes
Recipes are a great example of how shared knowledge can be meshed together. If recipes followed one or more common topics, like `recipes`, anyone could easily copy recipes and have them link into their recipes topic. Each recipe would be "a recipe named something in recipes". After creating and downloading a few, your folders might look like this:

```
me/private/notes/topic/recipes
me/private/notes/recipe/my grandmothers biscuits
markbittman/public/recipes/recipe/stuffed flank steak
michaelruhlman/public/recipes/recipe/east carolina barbecue
```

