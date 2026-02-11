---
title: StuPo Crawler
type: docs
prev: knowledge_file_gathering
next: pdf_file_combination
weight: 5
---
We have utilised the python package [beautiful soup](https://beautiful-soup-4.readthedocs.io/en/latest/) in order to automatically get information on all of the study programs. There are 144 study programs at the TU Berlin. Adding each of the study programs including any kind of detailed information by hand to the knowledge is not achievable in the extend of one semester. The python crawler that we have written allows us to scan through the list of study programs and gather information to each of them. It extracts the links to the study program websites and scans through them to find any kind of useful text. The script tries to maintain the structure of the webpage as well as possible, while combining the information of all study program websites in one markdown file. This markdown file is seperated by headings with the names of the study programs. 

The GitHub workflow executes the python crawler and uploads the generated markdown file. The crawler also downloads all available StuPOs and combines them into one large pdf. Unfortunately, the file is too large which leads to the chatbot hallucinating instead of properly accessing the correct StuPo. Future work could investigate how indexing can be used to improve the use of very large knowledge files. Due to the time constraint we decided to not persue this issue and to not include the StuPO pdf in our knowledge. This is why the workflow ignores the combined StuPO pdf file and does not upload it.

Utilising crawlers or scrapers to gather knowledge files plays a large role in the maintainability of a knowledge base. Eventually information will change. Having the option to gather all current information from the TUB websites by the press of a button is hugely beneficial to the maintainers of a chatbot.