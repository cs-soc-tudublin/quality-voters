# Quality Voters
This repository contains all the GitHub Actions, Workflows and other voters that CS++ use to ensure quality programs are developed.
For the sake of brevity, all of the above-mentioned items shall be called 'voters'

## Design Vision
Our aim is to have a small list of universal or extensible voters.
This will improve the Dx as less time is required to write custom voters for each project.
Minimal modifications should be required to these voters to make them applicable to your project.

## Wave 1 Voters
- SonarQube
- Spell Check
- File Existence Checks
- Link Resolution Checks

## Wave 2 Voters
- Container Build Checks
- Linting
- Accessibility
- Unit & E2E Test Runners