# SonarQube Voter
SonarQube is a code analysis tool that analyses the quality, format and security of code.

It provides a simple 'go/no go' system, AKA the voter passes if there are no issues, and fails if there are

## Configuration
> [!NOTE]
> Please read these instructions carefully, or SonarQube will not work correctly.

1. Log into SonarQube

2. Go to Projects and click 'Create Project', then select 'From GitHub'.

3. Select `cs-soc-tudublin` as the organisation.

4. Select the repository and import.

5. Select the 'Use the global setting' option during Project Setup, then select 'Create Project'.

6. Select 'With GitHub Actions' under the 'How do you want to analyze your repository?' header.

7. Follow the relevant instructions for adding. **EXCEPT!**

8. At the Create Workflow YAML file, select the correct option, BUT:

> [!IMPORTANT]
> These instructions must be followed correctly, or SonarQube will not correctly work!
- Create the `sonar-project.properties` file with the correct value.
- Add `sonarqube.yml` to `.github/workflows` in the repository INSTEAD of the generated one.
- Modify the `on`>`push`>`branches` branch to the relevant branch (main / master, or the development branch if branch protection is enabled.)