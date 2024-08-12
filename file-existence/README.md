# File Existence Voter

## Design Vision
The file exisence voter should check that all files that are referenced actually exist in that path. This prevents broken links to files by way of typo, directory mistake or non-existing file.
For .env or other files that should be excluded, there should be a file (maybe .gitignore?) that gives link exceptions for the voter to ignore.

The voter should run during a branch push, or a PR and fail if any links fail to resolve.