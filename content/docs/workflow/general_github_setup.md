---
title: General GitHub Setup
type: docs
prev: workflow
next: github_workflow
weight: 1
---

We quickly realised the value of version control. Even small changes in prompts and knowledge files can affect the quality of the chatbot answers. Using git as version control allows us to track all changes and revert to older versions in case the performance declines. A great help during the work with local git is the [online git documentation](https://git-scm.com/about).

To enable cooperative work on the chatbot sources and provide an easy to use webinterface we used GitHub as a git server provider. We have created a [TUNa repository](https://github.com/Themightyfirefly/TUna) that allows every contributer to pull the newest sources and push additional knowledge or other changes from their local computer to the server for everyone to use. Additionally, README files within the repository provide extra information on how to use the provided tools.