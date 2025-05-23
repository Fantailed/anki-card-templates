# Anki Random Substitution Card Types

These cards types are handy for adding a bit of variation into your sentence structure studies.  
Instead of learning the same fixed example sentence every time, these card types challenge you to understand and translate a general structure and even cycle through some vocabulary as well.

## Basic Random Substitutions

This card type allows you to create a card with placeholders that are substituted with a random values from given lists for each substitution slot.

Each substitution value is picked separately and randomly.

### Usage

* In the text field for the "Front" card, you can write `[[n]]` to create a placeholder, where `n` is a number starting from 0
* In the "Options" field, write all possible substitutions for placeholder `n` on line `n`, separated by a `|`
* The "Back" card and "Answers" fields work analogously.

### Example

```
Front
-----
The creature is [[0]] and [[1]].


Options
-------
small|big
furry|smelly
```

The resulting sentence will be a random one of these:
* The creature is small and furry.
* The creature is big and furry.
* The creature is small and smelly.
* The creature is big and smelly.


## Basic Random Fixed Substitutions

This card type works almost like [Basic Random Substitutions](#basic-random-substitutions), except all the substitutions are chosen together.

This can be useful if the different substitutions are related to each other.

### Example

```
Front
-----
This is my [[0]]. [[1]] is [[2]] than my [[3]].

Options
-------
mother|father
She|He
younger|older
father|mother
```

The resulting sentence will be a random one of these:
* This is my mother. She is younger than my father.
* This is my father. He is older than my mother.

Note how the different substitutions here should not be picked completely randomly but are always related to each other.  
This card type will ensure that e.g. all the first options are substituted together.
