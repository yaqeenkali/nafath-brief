Version: NAFATH-V4
Track: Cybersecurity

## Overview
A secure software supply chain requires trust in every component, from application code and third-party libraries to AI models, mobile apps, and internet routing. The Twelve-Factor App approach helps keep configuration separate from source code, reducing accidental exposure of credentials. AI security assessments identify attacks that manipulate training data or model inputs. OWASP MASVS provides a structured way to verify mobile application protections. Network operators can use RPKI-based route origin validation to reduce certain BGP hijacking risks. An SBOM records software components and their relationships, helping teams identify affected dependencies when vulnerabilities emerge. These controls complement one another: no single tool guarantees security across the entire supply chain. The Log4Shell incident demonstrates why vulnerability management and 
timely patching are essential.

## Software
The Twelve\-Factor App methodology emphasizes explicitly declaring software dependencies and keeping configuration separate from source code\. These practices are important because many applications rely on third\-party libraries that may contain vulnerabilities\. Declaring dependencies helps developers identify the components used in an application\. Separating configuration from source code also helps reduce the risk of exposing sensitive credentials in code repositories\. However, these practices should be supported by dependency scanning and effective secret management to strengthen software supply chain security\.

Resource: The Twelve\-Factor App \- III\. Config \- https://12factor\.net/config

## AI
Adversarial machine learning focuses on techniques used to manipulate or exploit AI systems. These include poisoning attacks that compromise training data, evasion attacks that cause incorrect predictions, and privacy attacks that attempt to infer sensitive information. Generative AI systems may also be vulnerable to misuse. Understanding these threats helps teams evaluate AI-related risks and implement suitable defenses. Security reviews should consider the data, models, and processes involved throughout the AI lifecycle.

Resource: Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2025/final

## Mobile
The OWASP Mobile Application Security Verification Standard &#40;MASVS&#41; defines security requirements for mobile applications\. It covers key areas such as secure storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy\. Development teams can use MASVS to establish security requirements and assess whether their applications meet them\. Combining these requirements with thorough security testing helps identify vulnerabilities and improve mobile application security before attackers can exploit weaknesses\.

Resource: OWASP Mobile Application Security Verification Standard &#40;MASVS&#41; \- https://mas\.owasp\.org/MASVS/

## Networking

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
