---
tags: a/note
---
in:: [[fractal knowledge]]

# Outstanding questions
## Disambiguation
One of the fundamental design questions for a knowledge format is how it handles [disambiguation](https://en.wikipedia.org/wiki/Wikipedia:Disambiguation), notes where the name can mean more than one thing.

Wikipedia's example is mercury, which can be an element, a god, or a planet. They differentiate through titles like "mercury (element)", "Mercury (planet)", and "Mercury (mythology)". Fractal knowledge intends to use note type in the same way, "a planet named mecury in planets."

With shared knowledge, the repository `owner` is the other main diambigation field, so even two different mercury notes by different people are distinct.

Is this a good approach? It's going to lead to thousands of note types. Will that scale, or lead to chaos.

## Global topics
Certain topics seem global in nature. Topics and repositories are the defined ones, but anything related to types of notes seems the same, 'a person in people', "a recipe in recipes". Should these be explicitly defined, or would this be trying to define common sense? One approach might be to let wikilink magic create the topic if it doesn't exist, and then apply the `topic` template to it. Or create one or more repositories with common types that could be imported.

## Note naming conventions
There are no rules around naming notes. That may make things incredibly messy when combining many repositories from many people. But the Obsidian quick switcher seems to search the full path, so typing the first couple of letter from the repository and note names narrows the list quickly. And a lot of nagivation will use topics or tags, so it might not matter how cluttered the namespace gets.

## Partial repositories
People might not want to pull in entire knowledge repositories when all they want is a single note. Like a recipes repository, they might only want their one or two favorites. The notes might then link to non-existant notes or topics that would exist if the entire repository were pulled in.

## Wikilinks to duplicate topics or notes
Using the recipes example again, everyone might publish recipes, but might also publish a `recipes` topic, which would conflict with your `recipes` topic. You might prefer your topic most of the time, but want to read others on occasion.

One potentially solution is to deliberately allow duplicate wikilinks, so when it occurs, you're presented with a menu to select the one you're interested in. A method to prefer "your" topics and notes, but allow selections of others would make for fairly seamless navigation.