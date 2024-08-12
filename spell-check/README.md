# Spell Check Voter

## Design Vision
The spell check voter should check HTML, Markdown, READMEs, etc. (any file which contains text that would be read by a user) and verify correct spelling.
For words specfic to the project, there should be a file which gives word exceptions for the voter to ignore.

The voter should run during a branch push, or a PR and fail if any typos are detected.