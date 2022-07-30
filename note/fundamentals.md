---
tags: a/note
---
in:: [[fractal knowledge]]

## Fundamentals
### Rulesets
Rulesets define how knowledge is organized. Like a card or board game, the rules tell you what to do. As long as you follow them, you can read other's people knowledge, and share your own with them.

Fractal knowledge is itself stored using a simple ruleset called the [[fractal knowledge core ruleset]], which combines notes into topics, topics into sharable knowledge repositories, repositories into a knowledge set. So it's both an explanation, and an example of how to use it.

More complex rulesets are planned in the future 😁!

### Knowledge repositories
Knowledge repositories are one of the fundamental building blocks. Anyone following a ruleset can create a knowledge repository that can be shared with others. Your knowledge will automagically link into the knowledge structure of anyone else following the same (or compatible) rules. It does this by publishing one or more topics, explained below

All knowlege repositories have an owner, level of sharing, and name. These are used when storing notes from that repository, so you know where all notes come from and how they should be treated.

### Sharing
Three levels of sharing are defined.
- Private: private notes are not shared
- Shared: notes shared with a limited number of people
- Public: notes are shared with all people.

Fractal knowledge can use any sharing method for knowledge repositories

### Topics
Topics organize notes, describing what the knowledge is about. If you've heard of "maps of content" (MOCs), it's the same thing

The core ruleset estabishes some fundamental topics like `topics` and `repositories`. The topics in knowledge repositories link into these special topics, and that's how the automagic linking happens. You can see this in action at the top of this file.

Topic can contain subtopics. All that means is that one topic links to another topic instead of the special `topics` topic.

### Notes
Notes hold knowledge in human-readable [markdown](https://help.obsidian.md/How+to/Format+your+notes) format. The Obsidian format includes wikilinks which are used here as the primary linking method.

Notes in fractal knowledge have a type. You've seen the two main ones: topics and notes, but other types are encouraged. Practical example include notes about a person, idea, thing, meeting, recipe. Type must be a singular noun.

### Index
The index is the starting place for your knowledge. You may gather lots of knowledge covering many topics. The index is a blank slate to link to your favorite knowledge.

As a note to those publishing knowledge repositories, don't mess with anyone's index, or even wikilink to it. This keeps backlinks clean so the user can decide how they want to link things.

### Tagging
The core ruleset uses the single nested tag `a`, along with the type of note. Notes are tagged `a/note`, topics are tagged `a/topic`, and so on. This makes searching easy, and doesn't interfere with other people's tag usage.

### Linking
All notes must link to a topic. Links use a special [inline field](https://blacksmithgu.github.io/obsidian-dataview/data-annotation/) named `in`, with wikilinks to one or more topics. For example, this note links to the fractal knowledge topic like, `in:: [[fractal knowledge]]`. This linking structure works well with backlinks and Obsidian plugins like dataview and breadcrumbs.

The `index` and `topics` notes are special, with their `in` fields pointing to each other for fast navigation.

### Referring to notes
You can refer to notes by their type, name, and topic. So this is "a note named fundamentals in fractal knowledge" A cooking note might be "a note named something in cooking"

### Storing notes
All notes are saved using the same naming convention, using four levels of folders.
- Owner: who owns the knowledge repositories inside this folder
- Sharing level: one of private, shared, or public
- Repository name: name of repository
- Type: type of note

So if you included this repository in your knowledge, this note would be stored at `digitalreplica/public/fractal knowlege/note/fundamentals`.

A default repository is defined and located at `me/private/notes`. It should be obvious that you own the notes, they're your private notes, not to be shared. Inside the repository, a note would go in the note folder, a topic will go in the topic folder.

This makes it easy to find all notes of a given type across all repositories, by searching like `/topic/`. 

### Templates
There are templates to make all this easier, but there's no convention (yet) for where to put them. It's assumed that many people will publish templates, so a similar naming convention to notes may be needed.

### Knowledge sets
All of these pieces combine into a knowledge set. This is simply a collection of knowledge repositories and a couple of special files.

You might want multiple knowledge sets when some knowledge can't be shared, like separate personal and work notes. Each knowledge sets would then have it's own private notes, but might share one or more repositories between them.
