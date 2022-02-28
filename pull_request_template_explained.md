# Pull Request template explained

## Branching
- If your PR is part of multi-PR effort - choose correct feature branch
- If your PR is one-PR change (bug fix or feature) use latest branch. This will usually be `develop`.

## Manual deployment

What does manual deployment mean?

Examples could be
- Creating a node
- Adding a block
- Running a drush command
- Adding a cron tab

The goal should always be to not have any manual deployment steps. If you can for example create a node in an update hook instead, that is always much better.

## Manual testing

What does manual testing mean?

If your task is to set a field upon updating a node, and you just altered the code so that it looks correct, please also make sure you try to actually save a node. Maybe you event want to try and save a couple of different node types.

If PR is towards a module repository used on several projects, please also specify which projects you have tested it on. If you need info on which projects are using this module, ask someone. Please also indicate which repository you tested on.
