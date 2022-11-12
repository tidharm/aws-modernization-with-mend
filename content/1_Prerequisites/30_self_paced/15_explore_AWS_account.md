---
title: "Get familiar with the architecture and AWS Resources"
chapter: false
weight: 15
---

Let's go over the architecture of our pipeline, get familiar with changes been made to your account and AWS services used.

### Reference Architecture

TBD: Add reference architecture and short description for each service

### CloudFormation template and resources needed to implement the architecture
So let's review what we are deploying:

- CodeCommit repository to host the application code
{{< importcode "../../static/CFN_Template.yml" 28 10 "yaml">}}

- CodeBuild project to run Docker and push the container image to ECR
{{< importcode "../../static/CFN_Template.yml" 40 21 "yaml">}}

- CodePipeline pointing to our CodeCommit repository and performing our CodeBuild and CodeDeploy actions
{{< importcode "../../static/CFN_Template.yml" 63 37 "yaml">}}

- Since CodePipeline does not automatically create this for you as part of creation, but this role is for the CWE Hook to trigger CodePipeline once there's an update in CodeCommit. Otherwise, we have to have CodePipeline poll for changes, which is slower.
{{< importcode "../../static/CFN_Template.yml" 106 19 "yaml">}}


### Get familiar with CodeCommit and CodeBuild configuration
Let's take a close look at Buildspec.yml structure - the configuration file for CodeBuild
{{< importcode "../../static/buildspec.yml" 0 25 "yaml">}}

### Let's do it! Deploying changes to your AWS account

Now when you are familiar with changes which will be made to you account, and you fill good about deploying it, let's run the Cloud Formation stack to create all resources needed. 

TBD 1-click link to CFN to run the template

{{% notice tip %}}
Since we use CloudFormation stack, it will be easy for you to remove it all once we done! You just need to delete the stack. No worries, we will remind you in the end.
{{% /notice %}}