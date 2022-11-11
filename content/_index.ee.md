---
title: "Minimizing Open Source Dependency Risks"
chapter: true
weight: 1
---


# Minimizing Open&nbsp;Source Dependency Risks
<br>
<!-- ![Partner Logo](/images/Mend-Logo_Dark_Horizontal_withTagLine.svg) -->
![Mend Logo](/images/Mend-Logo_Dark_Horizontal_withTagLine.svg)
<br>

## Introduction

Application developers are increasingly relying on open-source to deliver software at a faster pace, and open source now comprises over 70% of the typical application code base.  

At the same time, attacks on applications have increased. Today, applications are the #1 target and the biggest security risk that enterprise security teams face. The number of software supply chain attacks increased by 650% from 2020 to 2021.  

For these reasons, open source software needs to be secured. Join Mend in a hands-on virtual workshop where you’ll learn how to implement open-source security best-practices early in your workflow using AWS Development tools.  

You will have the opportunity to learn best practices for protecting your code early in the development life cycle with [Mend SCA](https://www.mend.io/open-source-security/) and save time and reduce risk by automating dependency updates in your software projects with [Mend Renovate](https://www.mend.io/free-developer-tools/renovate/) implemented inside your AWS development tools [AWS CodeBuild](https://aws.amazon.com/codebuild/) and [AWS CodeCommit](https://aws.amazon.com/codecommit/).  

## Learning Objectives
By the end of this workshop, you will be able to identify open-source security vulnerabilities in your code using [Mend SCA](https://www.mend.io/open-source-security/), and save time and reduce risk by automating dependency updates in your software projects with [Mend Renovate](https://www.mend.io/free-developer-tools/renovate/) from within your AWS development tools [AWS CodeBuild](https://aws.amazon.com/codebuild/) and [AWS CodeCommit](https://aws.amazon.com/codecommit/).  

## Audience
This workshop is intended for Developers, DevOps and AppSec champions and is particularly beneficial for those who are experienced with AWS Dev-Tools.  

## Workshop Structure
<ul>
    <li> Prerequisites and environment setup *(15 minutes)* </li>
    <li> Module 1: Integrating Mend SCA with CodeBuild *(15 minutes)* </li>
    <li> Module 2: Integrating Mend Renovate with CodeBuild *(15 minutes)* </li>
    <li> Module 3: Integrating Mend Renovate with CodeCommit *(15 minutes)* </li>
</ul>


{{% notice warning %}}
This workshop contains vulnerable code samples for training purposes.  
It is highly recommended to refrain from using your regular development/production environments for this workshop.  
Using your regular environments might trigger false alerts in your organization or result in security risks.  
Please consult your organization’s AppSec authority if you are uncomfortable with this matter.
{{% /notice %}}

[Let's get started!](/1_prerequisites.html)

<br>

# workshop.io REFERENCE

<br>

### Setting Up The Workshop: AWS Hosted Or Self-paced
By utilizing the Hugo language localization settings, directing the workshop towards a specific setup can be simplified. The `Language` setting in the `config.toml` file will allow you to distinguish between having one option or both. Commenting out one of the languages will hide all files that are related to that setup. By default, only the self-guided setup will be enabled. To enable switching, set `disableLanguageSwitchingButton` to `false` in the `config.toml`. If you want to have only the Event Engine setup, set the `defaultContentLanguage` at the top of the `config.toml` file to `ee`.

### The Entry Point Of The Workshop And Naming Conventions
All modifications should be done to files in the `content` folder. `_index.md` serves as the main entry point to your workshop. Adding modules can be done utilizing the format of `#_title` as a folder within `content`. By adding a number value to the title, this helps to keep the files structured in parity with the content of the workshop. A good practice for file naming is to have the folder be the module number and the submodule numbers add to that number reflecting their order. For example, the first module is `1_ModuleOne` and the submodules would be `11_SubmoduleOne`, `12_SubmoduleTwo`, and so forth. <br> <!-- <br> applies a line break to paragraphs -->
To ensure the modules and submodules follow the correct structure order, adjust the "weight" value in the heading of the file to reflect the order you wish to use. Three module examples are included in this template with the second being split based upon the method of setup. The same rules apply for submodules. `_index.md` will be the entry point of that module. Submodules should be named with the format of `{module number}{weight}_{title}.{language}.md`. For example, `11_Foreword.md` would be the first submodule of module one in the default language/setup. `31_PartnerSetup.ee.md` would be the first submodule of module 3 in the EventEngine language/setup.

### Working With Hugo Markdown and Shortcode
The following links will supply you with all the reference documentation about Hugo markdown. For more experienced developers, inline HTML is also an option to add more customization. For example `<p style='text-align: left;'>` inline will allow you to adjust your text placement.

### Markdown and Shortcode Resources
{{% notice tip %}}
The following links are your go-to resource for markdown and shortcode reference in building your workshop: <br>
* Markdown cheat sheet https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet <br>
* Learn theme markdown https://learn.netlify.app/en/cont/markdown/ <br>
* Menu extras and shortcuts https://learn.netlify.app/en/cont/menushortcuts/ <br>
* Using Font Awesome Emoji's <i class="fas fa-heart"></i> https://learn.netlify.app/en/cont/icons/ to help your page pop <i class="fas fa-glass-cheers"></i>
{{% /notice %}}

### Adding Images and Static Media
Any images and static media to be included in the workshop need to be placed in the `static/images` folder. The format to display an image is as follows: `![Alternate Text](/images/imagename.jpg)` <br>

For example, the markdown for this dog is `![AWS Logo](/images/AWS_Logo.png)` and the image is in the `static/images` folder. <br>
![AWS Logo](/images/AWS_Logo.png)

### Creating Links
The format for creating links is `[Link Display Text](http://example.com)`. For example, this link [Hugo Framework](https://gohugo.io/about/what-is-hugo/) was created using `[Hugo Framework](https://gohugo.io/about/what-is-hugo/)`.

### The "More" Menu Section
This section of the menu on the left is designed to add additional resources that are related to the workshop but not necessarily part of the workshop itself. To modify these links, edit the sections marked `[[menu.shortcuts]]` in the `config.toml` located in the root folder. The "name" portion will be what is displayed in the menu. The "url" should be the address of the link. The "weight" setting will adjust the display order, similar to the other "weight" settings utilized in indexes and modules mentioned previously.

### Ensuring Pages Appear In Both Setup Versions
A shortcut to creating the workshop with different setup versions is utilizing the localization functionality of Hugo. By adding a secondary extension to the filename, this file will be included in the specific version of the workshop. Currently, the base utilizes the format `*.ee.md` to signify that the page is to be used in the AWS EventEngine setup. Much of the time, the files will be the same as the content only differs at specific points. It is necessary to add them, however, to make sure that the common content is duplicated across both versions. If you wish to change the secondary extension or default version, this can be done in the `config.toml` file in the heading and `[Languages]` sections.