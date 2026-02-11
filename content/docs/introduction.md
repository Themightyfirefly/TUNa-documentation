---
title: Introduction
next: docs/chatbot_design
type: docs
weight: 1
---

Universities rely on complex and widely distributed digital infrastructures to manage study organization, academic regulations and other administrative processes, with the intention of providing transparency and enabling self service. While these systems have distinct use cases, they also result in a highly fragmented and scattered information network for students. This can be also seen at TU Berlin, where information on exams, course registrations, study regulations and other advisory services are spread across multiple platforms and documents. Producing difficulties for students to quickly find and identify relevant answers in their everyday student organization.

This project addresses these challenges through the development of TUNa (TU Navigator), a GPT-based, domain specific chatbot designed to support students in organizing their studies at TU Berlin. TUNa aims to centralize access to study related information by providing reliable answers to frequent student queries.

The scope of this helper is intentionally limited to study related organizational processes at the TU Berlin, which include the topics of examinations, course and exam registrations, thesis submission, study regulations, learning platforms such as ISIS and MOSES, Erasmus programs and relevant administrative contacts and locations. By design choices, topics outside of this domain are deliberately excluded to reduce ambiguity and prevent hallucinations to ensure that the responses are grounded and verified.

The intended use case of TUNa is to serve as a information and organizing assistant for student of TU Berlin, who need quick and reliable information without first browsing multiple different university websites or contacting administrative offices for their questions. The chatbot is not intended to replace official advisory services but to complement them.

The primary project goal is to evaluate whether a carefully scoped, GPT-based chatbot can reduce the time and effort students spend searching for study related information while maintaining a high level of correctness and trustworthiness. A secondary goal is exploring how prompt engineering techniques, such as role prompting, selective clarification, and verification driven reasoning, can be combined to achieve robust model behavior in a high stakes, administrative domain. Accordingly, this report documents both the technical design decisions and the empirical evaluation of the system’s effectiveness compared to a general purpose GPT baseline.