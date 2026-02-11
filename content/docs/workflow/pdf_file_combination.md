---
title: PDF File Combination
type: docs
prev: stupo_crawler
next: future_use
weight: 6
---

To aid flexibility and maintainability of the gathered pdf resources, we created a [python script](https://github.com/Themightyfirefly/TUna/blob/main/General_Scripts/combine_pdfs.py) that combines all pdf files within a given directory. Inside the script, a maximum file size is defined. This can be used to prevent knowledge files from getting too large. The script will combine all pdf files in the given directory into as few files as possible while maintaining the maximum file size. 

The script is executed by the GitHub workflow, which applies the script to all directories that include "combine_" in their name. An example for how to utilise this tool can be found in the Erasmus knowledge. Here, brochures including all faculties' exchange cooperations have been downloaded from the TU Berlin website and copied into a directory called [combine_Incoming_Erasmus_Brochure](https://github.com/Themightyfirefly/TUna/tree/main/Knowledge/Exchange_Students/combine_Incoming_Erasmus_Brochure). On execution the GitHub workflow will combine all of these brochures into one pdf file called "Incoming_Erasmus_Brochure.pdf". By utilising this tool, we are able to reduce the number of knowledge files, while keeping the pdf knowledge files customisable.