+++
title = "Cleanup"
chapter = true
weight = 170
+++

## Cleanup
{{% notice note %}}
If you are attending AWS Event and using one of provided AWS accounts than you can skip this section.
{{% /notice %}}

If you used the provided CloudFormation template, the cleanup is easy! 

* Navigate to *CloudFormation -> Stacks*, select *`MendWorkshop`* stack
* Switch to *Resources* tab, and find `CodePipelineArtifactBucket` Logical ID (the S3 bucket used to store CodePipeline logs). Click on the Physical ID link. It will open the S3 bucket in the new tab
* Select all content (use the top checkbox in the first column on the left) and click **Delete** button. Type *`permanently delete`* and confirm with **Delete objects** button
* Navigate back to the browser tab with CloudFormation template open, and click **Delete** button for the stack, confirm by **Delete stack** button. It will take a little time and all workshop resources will be removed!

Thank you for learning with us!