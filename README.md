# Loom: A dialogue system for {your_game}
Loom is a dynamic dialogue library for games with inline lisp-like expressions!

## Features
### Writeable syntax
Loom is written like a roleplaying script and requires very little boilerplate, for example:
```
Loom: This is an example of dialogue!
You: Seems pretty intuitive.
```

### Inline expressions
Write inline dynamic expressions like `(log {player_name})` for programatic behavior.

### Variables
Variables can be read from and written to in dialogue and expressions via the `{varName}` accessor syntax.

### Choices
Branching dialogue is as simple as calling the `->` function in an expression to add a user-exposed choice to the interaction:
```
Loom: Do you think my arrow syntax is cool?
(-> "Yes." (
    Loom: Glad to hear it!
))
(-> "Not really." (
    Loom: Aw, you're too sweet.
))
```
