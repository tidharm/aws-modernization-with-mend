---
title: "Launch Cloud9 IDE Workspace"
chapter: false
weight: 10
---

{{% notice info %}}
This section is optional. If you have local IDE where you can format YAML files and explore code as needed, you can skip it and move to the next section.
{{% /notice %}}

[AWS Cloud9](https://aws.amazon.com/cloud9/) is a cloud-based integrated development environment (IDE) that let you write, run, and debug your code with just a browser. It includes a code editor, debugger, and terminal. Cloud9 comes prepackaged with essential tools for popular programming languages, so you don’t need to install your own to edit files or configuration.

We will use Amazon Cloud9 to access our AWS account via the AWS CLI in this workshop, modify build configuration and more. There are a couple steps to access it:

 - Navigate to the [Cloud9 console](https://console.aws.amazon.com/cloud9/home) or just search for it under the **AWS console services** menu
 
 - Run pre-deployed **aws-workshop** Cloud9 environment 

### Configure Cloud9 IDE environment

When the environment comes up, customize the environment by:

1. Close the **welcome page** tab

2. Close the **lower work area** tab

3. Open a new **terminal** tab in the main work area.

4. Hide the left-hand environment explorer by clicking on the left side **environment** tab.

{{% notice tip %}}
If you don't like this dark theme, you can change it from the **View / Themes** Cloud9 workspace menu.
{{% /notice %}}

{{% notice tip %}}
Cloud9 requires third-party-cookies. You can whitelist the [specific domains]( https://docs.aws.amazon.com/cloud9/latest/user-guide/troubleshooting.html#troubleshooting-env-loading). Ad blockers, javascript disablers, and tracking blockers should be disabled for the cloud9 domain, or connecting to the workspace might be impacted.
{{% /notice %}}

<!-- uncomment if needed
 Now we will attach the proper role to our Cloud9 EC2 instance and configure a bit more our Cloud9 environment:

{{% notice info %}}
Cloud9 normally manages IAM credentials dynamically. This isn't currently compatible with
the EKS IAM authentication, so we will disable it and rely on the IAM role instead.
{{% /notice %}}

- [Attach the IAM role to your workspace](/15_workspace_setup/152_workspaceiam.html)
- [Configure workshop specific requirements](/15_workspace_setup/153_cloud.html)
-->
