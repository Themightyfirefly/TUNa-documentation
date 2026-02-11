---
title: Knowledge File Gathering
type: docs
prev: chatbot_settings_and_prompt_deployment
next: stupo_crawler
weight: 4
---


The previously discussed workflow gathers knowledge files and provides them as a combined zip archive. In order to do so, it follows these rules:

- Gather all file paths within the [**Knowledge directory**](https://github.com/Themightyfirefly/TUna/tree/main/Knowledge)
- **Exclude python files** and their requirements.txt files
- **Exclude files or directories** with the following keywords in their name or path 
    - "**combine_**", as such directories will be used for pdf combining. 
    - "**survey**", as any survey related documents should not be part of the knowledge
    - "**StuPos**", as the generated combined StuPo is currently too large

This leaves the workflow with all of our markdown, pdf and json files which it can copy into a temporary directory. The directory with all of these knowledge files is then uploaded as an artifact and provided as a download to the user within the GitHub actions tab.