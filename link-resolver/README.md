# Link Resolution Voter

## Design Vision
The link resolution voter should check all files for a URL by means of a regular expression (Except for localhost URLs) and ensure they actually resolve. This prevents broken links being introduced.
For localhost or other links that should be excluded, there should be a file that gives link exceptions for the voter to ignore.

The voter should run during a branch push, or a PR and fail if any links fail to resolve.