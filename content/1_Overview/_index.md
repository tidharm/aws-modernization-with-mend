---
title: "Overview"
chapter: true
weight: 1
---

# Overview

## Open Source Software Security Issues

Open source software is software that someone else wrote — not your own developers. The author of the open source software typically wraps their code into a "package" and publishes it on the Internet for other people to download and use.

Here's a great video about open source software: [The Rise of Open-Source Software](https://www.youtube.com/watch?v=SpeDK1TPbew)

When an application relies on an open source package to perform some function, the open source package is known as a "dependency". From a security point of view, it is important to know that there are two kinds of dependencies:

* **Direct Dependency** - third-party code that was knowingly added to the application by its developer.
* **Transitive Dependency** - third-party code that was added to the application by another direct dependency. In most cases, the developer will not be aware of this code unless they utilize a designated tool or method, such as software composition analysis, to list and identify all the application's direct and transitive dependencies.

The diagram below depicts the relationship between direct and transitive dependencies. As you can see, there are typically many more transitive dependencies in an application than there are direct dependencies, and vulnerabilities can manifest in both direct and transitive dependencies.


![](/images/overview/direct_transitive.png)


A **Software Composition Analysis (SCA)** tool can list and identify both direct and transitive dependencies in your application, and can provide information and remediation suggestions for them, so you can address them before they have any reputational, IP or monetary impact.

### The Rising Incidence of Vulnerabilities in Open Source Software
Open source software is always open for everyone to see – both developers and hackers.  
New vulnerabilities are constantly being identified in open source software, and once a vulnerability becomes public knowledge, it's only a matter of time before bad actors will target that code and try to exploit it.

Here are a few examples of famous open source software vulnerabilities:

- **[The Heartbleed Bug (CVE-2014-0160)](https://www.mend.io/vulnerability-database/CVE-2014-0160)**  
A vulnerability that was [discovered](https://heartbleed.com/) in 2014 in [OpenSSL](https://www.openssl.org/) and resulted in several massive data breaches, including the [famous data breach](https://www.healthcareitnews.com/news/hackers-exploit-heartbleed-swipe-data-45-million#:~:text=In%20the%20second%20biggest%20HIPAA,snatched%20by%20cybercriminals.) of 4.5 million people held by Community Health Systems.  
- **[Apache Struts (CVE-2017-5638)](https://www.mend.io/vulnerability-database/CVE-2017-5638)**  
A vulnerability that was discovered in 2017 in [Apache Struts](https://struts.apache.org/announce-2017.html), a vulnerability through which [Equifax suffered a massive breach](https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/) the same year.
- **[Log4Shell (CVE-2021-45046)](https://www.mend.io/vulnerability-database/CVE-2021-45046)**  
A vulnerability that was [discovered](https://www.mend.io/resources/blog/log4j-vulnerability-cve-2021-45046/) in 2022 in [Apache Log4j 2](https://logging.apache.org/log4j/2.x/), a popular Java library for logging error messages in applications, and caused several government agencies to be easily breached.  

These are only a few famous examples. Each year, thousands of open source software vulnerabilities are discovered, as depicted in the following graph:

![](/images/overview/oss_vuln_per_year.png)


Once a vulnerability has been announced, the developer (or the developer community) responsible for supporting the affected package will usually publish an update that fixes the vulnerability.  
But sometimes, this is not done, in which case, the developer of the application that uses the affected package can either switch to an alternative open source package that provides similar functionality but without the vulnerability, or mitigate the risk via another approach.

Now, let’s see how you can integrate a highly effective software composition analysis tool with your development toolchain, that will help you identify and remove open source software vulnerabilities in your application.

### [Let's get started!](/2_prerequisites.html)
