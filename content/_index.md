---
title: "Minimizing Open Source Dependency Risks"
chapter: true
weight: 1
---


# Minimizing Open&nbsp;Source Dependency Risks
<!-- <br> -->
<!-- ![Mend Logo](/images/Mend-Logo_Dark_Horizontal_withTagLine.svg) -->
![Mend Logo](/images/Mend-Logo_Dark_Horizontal.svg)
<!-- <br> -->

## Introduction

**[AWS Developer Tools](https://aws.amazon.com/products/developer-tools/)** were designed to support the rapid development of cloud native applications. They help maximize developer productivity by automating CI/CD pipelines.

But maintaining code security is your responsibility.

Fortunately, you can now add application security to the AWS Developer Tool workflow. Doing that lets developers efficiently find and fix many of the security vulnerabilities that inadvertently creep into their code.

This workshop will teach you how to add open source software security testing to an AWS Developer Tool chain. The advantages of this approach, as opposed to the traditional method of using separate security tools to test applications after they are built, are:

- **More Efficient Workflow**  
Security vulnerabilities are identified as soon as the developers commit their code. No waiting for test results.  

- **More Efficient User Interface**  
Developers see security alerts right in their native development environment. No need to run separate tests with non-integrated security tools.  

- **The 80/20 Rule**  
Typically, 80% of an application is comprised of open source software, and vulnerabilities can be easy to fix if a developer has the right information at the right time.  

This workshop will start with an overview of the security issues that plague modern cloud-based applications, including:  

- The rising incidence of serious vulnerabilities in open source software  
- Examples of attacks that leverage open source software vulnerabilities  
- The problem of vulnerabilities in transitive dependencies  

Next, you will learn how to implement security tools within the AWS development environment to address open source software security vulnerabilities quickly and efficiently.  
You will also learn how to efficiently keep your dependencies up-to-date with the world’s most popular tool: **[Mend Renovate](https://www.mend.io/free-developer-tools/renovate/)**.  


## Learning Objectives
- Understand the security problems associated with open source software
- Learn how to efficiently identify open source software vulnerabilities early in the software development lifecycle, by adding [Mend SCA](https://aws.amazon.com/marketplace/seller-profile?id=14809865-492e-4295-8a12-288535dfea55) to your [AWS CodeBuild](https://aws.amazon.com/codebuild/) build pipeline.
- Learn how to save time automating dependency updates by adding [Mend Renovate](https://www.mend.io/free-developer-tools/renovate/) to your AWS development toolchain.

## Audience
This workshop is intended for Developers, DevOps and AppSec champions and is particularly beneficial for those who are using or planning to implement [AWS Developer Tools](https://aws.amazon.com/products/developer-tools/).  

## Workshop Structure
- Overview of open source software security issues *(6 minutes)*
- Prerequisites and environment setup *(TBD minutes)*
- Module 1: Integrating **Mend SCA** with **AWS CodeBuild** *(TBD minutes)*
- Module 2: Integrating **Mend Renovate for CodeCommit** with **AWS CodeBuild** *(TBD minutes)*

{{% notice warning %}}

This workshop contains vulnerable code samples for training purposes.
It is highly recommended to refrain from using your regular development/production environments for this workshop.
Using your regular environments might trigger false alerts in your organization or result in security risks.
Please consult your organization’s AppSec authority if you are uncomfortable with this matter.
{{% /notice %}}

<hr>

<!-- ### [Let's get started!](/2_prerequisites.html) -->
