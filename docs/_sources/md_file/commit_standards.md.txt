# Commit Standard Documentation

## Brief Introduction

This documents should be referred, when contributers want to commit messages. It provides an easy set of rules for creating an explicit commit history, which makes the purpose of commits more specific. 

The commit should be structured as follows:

> \<`type`\>[optional `scope`][optional `!`]: \<`description`\>

## Structural Elements 

Contributers can use the following elements to replace `type`, `scope` and `description`.

### Type

- **feat**: Introduce a new feature to the codebase (this correlates with MINOR in Semantic Versioning).
- **fix**: Patch a bug in your codebase (this correlates with PATCH in Semantic Versioning).
- **docs**: Make changes in documentation.
- **style**: Commit changes of code style, formatting, missing semicolons or whitespaces.
- **refactor**: Make code changes that neither **feat**(add a new feature) nor **fix**(fix a bug).
- **perf**: Commit changes that improve performance.
- **test**: Add missing tests.

### Scope(optional)

A scope may be provided to state the scope of commit's influence, to provide additional contextual information and is contained within parenthesis. 

For repository [MatchBench](https://github.com/ruc-datalab/MatchBench), we can use "dataset", "evaluator", "model", "pair_gen", "trainer", "utils" to state the scope of influence according the structure of MatchBench([ref](https://github.com/ruc-datalab/MatchBench/tree/main/matchbench)).

### Breaking Changes of !

Append a **!** after the type/scope, which introduces a breaking API change (correlating with MAJOR in Semantic Versioning).

### Description

The description contains a concise sentence of the applied changes. It has no specific standard, but we recommend to refer to the historical commits of corresponding repository.

## Commit Examples

Here, several commit examples of project [MatchBench](https://github.com/ruc-datalab/MatchBench) are given for better understanding.

> `feat`(`model`): `add an EA model RREA`

This means the commit adds an EA method to the submodule ["model"](https://github.com/ruc-datalab/MatchBench/tree/main/matchbench/model).

> `fix`(`trainer`): `fix bugs in base_trainer.py`

This means the commit is mainly about fixing bugs of base_trainer.py in submodule ["trainer"](https://github.com/ruc-datalab/MatchBench/tree/main/matchbench/trainer).

> `style`(`evaluator`): `tweaked the code of metrics.py`

This means the commit is mainly about code style tweak of metrics.py in submodule ["evaluator"](https://github.com/ruc-datalab/MatchBench/tree/main/matchbench/evaluator).

> `refactor`(`model`)<font color=red>!</font>: `call 'load_source_target' function before training`

This means we change the structure of all models in submodule ["model"](https://github.com/ruc-datalab/MatchBench/tree/main/matchbench/model). When building the model, we should call the function 'model.load_source_target()' before training process. The exclamation mark "!" is added to draw the attention of Project Manager.

## Reference
[1] https://www.conventionalcommits.org/en/v1.0.0/<br>
[2] https://github.com/jochaes/Picturess/wiki/Commit-Standard<br>
[3] https://github.com/anthoninCL/Flutter-I-MyTinder/wiki/Commit-standard<br>