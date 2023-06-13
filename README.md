# Azure Infrastructure As Code Workshop Content

## Overview

This repository contains labs to help people learn how to write and work with infrastructure as code in Azure. If you're new to Infrastructure as Code, start by reviewing the following [IaC concepts](https://learn.microsoft.com/en-us/training/modules/introduction-to-infrastructure-as-code-using-bicep/?ns-enrollment-type=learningpath&ns-enrollment-id=learn.bicep-deploy-manage).

Custom labs, open-hack style challenges and other content will be added overtime.

> *Note:* Currently the repository only provides learning guidance for developing IaC in Bicep using related Microsoft tooling.

<br>

# Content

### Visual Studio Code

| Lab | Overview | Link |
| -- | -- | -- |
| Tooling with Visual Studio Code | Learn how to install and configuration of Visual Studio Code. Then walk through cloning a git repository using VSCode | [VSCode Overview](https://learn.microsoft.com/en-us/training/modules/introduction-to-visual-studio-code/) <br> [VsCode Setup](https://code.visualstudio.com/Docs/setup/setup-overview) <br>  [Git Install](https://github.com/git-guides/install-git) <br> [VsCode Extensions](https://code.visualstudio.com/learn/get-started/extensions) |

## Bicep

> *Note:* If you're new to IaC follow the labs based on their order in the table.

## Fundamentals
| Lab | Overview | Link |
| -- | -- | -- |
| Introduction to Bicep Templates | Define Azure resources within a Bicep template. Improve the consistency and reliability of your deployments, reduce the manual effort required, and scale your deployments across environments. Your template will be flexible and reusable by using parameters, variables, expressions, and modules. | [Lab Part 1](https://learn.microsoft.com/en-us/training/modules/introduction-to-infrastructure-as-code-using-bicep/) <br> [Lab Part 2](https://learn.microsoft.com/en-us/training/modules/build-first-bicep-template/) |
| Build Reusable Bicep Templates by using Parameters | Use Bicep parameters to provide information for your template during each deployment. Add decorators to make your parameters easy to understand and work with, and to protect secret data. Provide parameter values at the command line and by using parameter files. | [Lab](https://learn.microsoft.com/en-us/training/modules/build-reusable-bicep-templates-parameters/) |
| Build flexible Bicep Templates by using Conditions and Loops | Deploy resources only when specific constraints are in place. Use loops to deploy multiple resources that have similar properties. | [Lab](https://learn.microsoft.com/en-us/training/modules/build-flexible-bicep-templates-conditions-loops/) |
| Create composable Bicep files using modules | Design and build reusable modules to simplify your Bicep templates. Compose multiple modules into templates by using parameters and outputs. | [Lab](https://learn.microsoft.com/en-us/training/modules/create-composable-bicep-files-using-modules/) |

## Intermediate

| Lab | Overview | Link |
| -- | -- | -- |
| Deploy child and extension resources | Deploy a variety of Azure resources in your Bicep code. Define and use child and extension resources. Work with resources that you created outside a Bicep template or module. | [Lab](https://learn.microsoft.com/en-us/training/modules/child-extension-bicep-templates/) |
| Structure Bicep for Collaboration | Build Bicep files that support collaborative development and follow best practices. Plan your parameters to make your templates easy to deploy. Use a consistent style, clear structure, and comments to make your Bicep code easy to understand, use, and modify. | [Lab](https://learn.microsoft.com/en-us/training/modules/structure-bicep-code-collaboration/) |
| Manage changes to your Bicep code by using Git | Track of changes to your Bicep code and view the history of the files you've changed. Use branches to develop multiple versions of your code at the same time. Publish your repository to support collaboration. | [Lab](https://learn.microsoft.com/en-us/training/modules/manage-changes-bicep-code-git/) |
| Review Azure infrastructure changes by using Bicep and pull requests | Avoid unintended changes and poorly written Bicep code by using pull requests. Use branching strategies to protect your main branch from accidental changes. Understand what you should look for when you review Bicep code. | [Lab](https://learn.microsoft.com/en-us/training/modules/review-azure-infrastructure-changes-using-bicep-pull-requests/)
| Preview Azure deployment changes by using what-if | Preview the effects of your deployments. Understand the types of changes detected by the what-if operation. Deploy your templates using incremental and complete mode.|  [Lab](https://learn.microsoft.com/en-us/training/modules/arm-template-whatif/)|
| Migrate Azure Resources and ARM templates to Bicep | Export and convert your Azure resources to Bicep files, and migrate your JSON Azure Resource Manager templates (ARM templates) to Bicep. Refactor your Bicep files to follow best practices. Test your Bicep files and deploy them to production. | [Lab](https://learn.microsoft.com/en-us/training/modules/migrate-azure-resources-bicep/) |

## Advanced
| Lab | Overview | Link |
| -- | -- | -- |
| Deploy resources to subscriptions, management groups and tenants | Deploy Azure resources at the subscription, management group, and tenant scope. Understand how Azure resources are deployed at different scopes, why this is important, and how to create Bicep code to deploy them. Create a single set of Bicep files that you can deploy across multiple scopes in one operation. | [Lab](https://learn.microsoft.com/en-us/training/modules/deploy-resources-scopes-bicep/) |
| Extend Bicep using deployment scripts | Add custom steps to your Bicep or JSON Azure Resource Manager templates (ARM templates). Integrate deployment scripts with your deployment by using parameters and outputs. | [Lab](https://learn.microsoft.com/en-us/training/modules/extend-resource-manager-template-deployment-scripts/) |
| Shared Bicep modules by using a private registry | Reuse Bicep modules to reduce code duplication and increase the quality of your deployments. Create a private registry for your organization. Publish shared modules to the registry, and consume them in multiple deployments. | [Lab](https://learn.microsoft.com/en-us/training/modules/share-bicep-modules-using-private-registries/) |
| Publish Libraries of reusable infrastructure as code using template specs | Reuse and share your ARM templates across your organization. Publish template specs that deploy resources pre-configured for your organization's requirements. Control access and safely update template specs by using versions. | [Lab](https://learn.microsoft.com/en-us/training/modules/arm-template-specs/) |


<br>

### CICD Tools

| Lab | Overview | Link |
| -- | -- | -- |
| Azure DevOps | Gain all of the benefits of infrastructure as code by using an automated pipeline to deploy your Bicep templates, and integrate other deployment activities with your pipelines. You'll build pipelines using Azure Pipelines. | [Lab](https://learn.microsoft.com/en-us/training/paths/bicep-azure-pipelines/) |
| GitHub Actions | Gain all of the benefits of infrastructure as code by using an automated workflow to deploy your Bicep templates, and integrate other deployment activities with your workflows. You'll build workflows using GitHub Actions. | [Lab](https://learn.microsoft.com/en-us/training/paths/bicep-github-actions/) |
| Defender for DevOps | Learn how to leverage the new Defender For DevOps tool to securely protect and scan your Infrastructure as Code. | [GitHub Lab](https://github.com/Azure/Microsoft-Defender-for-Cloud/blob/main/Labs/Modules/Module%2015%20-%20Integrating%20Defender%20for%20DevOps%20with%20GitHub%20Advanced%20Security.md) <br> [Azure DevOps Lab](https://github.com/Azure/Microsoft-Defender-for-Cloud/blob/main/Labs/Modules/Module%2014-Config%20Azure%20ADO%20in%20DfD.md)

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
