---
title: Chatbot Design
type: docs
prev: introduction
next: knowledge_format
weight: 2
sidebar:
  open: true
---

This section presents the overall design of the TUNa chatbot, outlining the core architectural decisions and conceptual principles that guided the development. The design focuses on achieving reliable, domain specific assistance for study organization at TU Berlin while addressing known limitations of large language models, such as hallucinations and sensitivity to ambiguous input. To this end, the chatbot combines a GPT-based language model with a curated knowledge base and a carefully engineered system prompt. The following subsections describe how knowledge is structured, how prompts are designed and iteratively refined, and how these components interact to produce consistent, trustworthy responses aligned with the intended scope and use case of the system.
