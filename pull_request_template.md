## Ny Media Pull Request Checklist (NMPRC)

### All code, documentation, and commits are in English.
- [ ] Yes, I have looked through the changes and find no traces of non-english.
- [ ] Some parts are not in english (please specify reason)

### Does the changes add any sensitive information
- [ ] No, no sensitive information in here.
- [ ] Some sensitive information in this PR (please specify what, and why)

### Does the changes introduce fields or otherwise make it possible to store new sensitive information?
- [ ] No, not sensitive or not relevant
- [ ] This makes it possible to store sensitive information

### If the change introduces storing sensitive information, are sanitization rules updated for it?
- [ ] No relevant
- [ ] Yes, they are updated
- [ ] No, they are not updated (please specify why not)

### Does the change include all translations for new strings?
- [ ] Yes, all strings are exported and translated.
- [ ] No, not all strings are translated or can not be translated (please specify why)
- [ ] Not relevant

### Did you use the correct branch based on rules below?
- [ ] If this is part of multi-PR effort - choose correct feature branch
- [ ] If this is a one-PR change (bug fix or feature) use current branch

### Does it require manual deployment? List manual deployment steps in the "Additional info" section below

<details>
<summary>What does manual deployment mean?</summary>

Examples could be
- Creating a node
- Adding a block
- Running a drush command
- Adding a cron tab

The goal should always be to not have any manual deployment steps. If you can for example create a node in an update hook instead, that is always much better.
</details>

- [ ] Yes, this requires manual deployment
- [ ] Not, this does not require manual deployment

### Did you manually test the change?

<details>
<summary>What does manual testing mean?</summary>

If your task is to set a field upon updating a node, and you just altered the code so that it looks correct, please also make sure you try to actually save a node. Maybe you want to save a couple of different node types even.
</details>

- [ ] Yes, I manually tested my changes
- [ ] No I did not manually test my changes (please specify why)

### List steps taken for own manual testing

Please fill in here

### Did you manually test the change in another project's repository?

Only applicable if this PR is towards a module repository used on several projects. Please also specify which projects you have tested it on. If you need info on which projects are using this module, ask someone. Please also indicate which repository you tested on.

- [ ] Yes indeed. I tested the change on another repository.
- [ ] No I did not
- [ ] Not relevant

Which repository?
n/a.

## Additional Info

Are there any links to specifications, references from correspondances or similar that is relevant? Please add them here.

## Instructions for testing

<details>
<summary>What does Instructions for testing mean?</summary>

One such recipe would be to list the steps to deploy this branch locally, and the steps needed to test that the PR does what it is supposed to. For example:

- Run `composer build`
- Log in as a user with "adminster nodes" permission
- Edit a node of type "article" and click "Save"
- The node should now have changed in some way.

</details>

If you have suggestions for how this Pull Request Template can be better, please create an issue (or a pull request) on [https://github.com/nymedia/.github](https://github.com/nymedia/.github)
