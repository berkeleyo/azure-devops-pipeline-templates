
# Azure DevOps Pipeline Templates

Reusable YAML templates for **Bicep builds** and **PowerShell module testing**.

## Use in your pipeline
```yaml
resources:
  repositories:
    - repository: templates
      type: github
      name: berkeleyo/azure-devops-pipeline-templates
      ref: refs/heads/main

extends:
  template: templates/iac-ci.yml@templates
  parameters:
    solutionPath: infra/
```
