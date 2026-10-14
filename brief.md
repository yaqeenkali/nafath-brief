Version: NAFATH-V4
Track: Cybersecurity

## Overview
Software supply chain security protects software throughout development, testing, distribution, and deployment\. Modern applications depend on third\-party libraries, development tools, infrastructure, and external services, so a weakness in one component can create risks for many users\. Software security helps developers manage dependencies and protect application configuration\. AI security addresses attacks against machine\-learning systems and their data\. Mobile security helps protect applications, devices, and sensitive information\. Network security supports reliable communication and reduces certain routing threats\. Cybersecurity practices help organisations identify vulnerabilities, manage access, and respond to incidents\. Software supply chain data, including a Software Bill of Materials &#40;SBOM&#41;, helps identify components and assess exposure to known vulnerabilities\. These areas work together to improve visibility and reduce risk\. This brief focuses on the cybersecurity question of how organisations can identify vulnerable software dependencies and ensure that security fixes are applied.

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
The Border Gateway Protocol &#40;BGP&#41; allows networks to announce IP address prefixes they can route to\. Incorrect or malicious announcements can redirect traffic or make destinations unreachable\. Resource Public Key Infrastructure &#40;RPKI&#41; supports route origin validation by allowing network operators to check whether an autonomous system is authorized to announce a particular prefix\. Although this provides an additional layer of security against certain routing risks, it does not validate the entire network path or prevent all routing attacks\. Therefore, operators must also implement appropriate routing policies\.

Resource: RFC 6811: BGP Prefix Origin Validation \- https://www\.rfc\-editor\.org/rfc/rfc6811\.html

## Cybersecurity
Log4Shell &#40;CVE\-2021\-44228&#41; is a critical remote code execution vulnerability affecting the `log4j-core` component of Apache Log4j 2\. Under vulnerable conditions, attacker\-controlled log messages can trigger unsafe Java Naming and Directory Interface &#40;JNDI&#41; lookups, potentially enabling remote code execution\. The vulnerability received a CVSS score of 10\.0, reflecting its critical severity\. Organisations should identify affected components, check their versions, and apply appropriate security updates\. Maintaining an accurate inventory of software dependencies helps teams identify potentially affected applications and prioritise investigation and remediation\.

Resource: Security \- Apache Logging Services \- https://logging\.apache\.org/security\.html
 
## Data
A Software Bill of Materials (SBOM) is a formal record of software components and their relationships. It helps organisations identify third-party libraries and assess potential vulnerabilities in their products. According to NTIA guidance, an SBOM should include the supplier name, component name, component version, other unique identifiers, component relationships, the SBOM author, and a timestamp. Machine-readable SBOMs can support automated analysis and improve vulnerability management. However, an SBOM provides an inventory of software components; it does not guarantee that the software is secure or free from vulnerabilities.

Resource: The Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

## Misconception in My Track
A common misconception is that all applications using Log4j are vulnerable to CVE-2021-44228. However, Apache clarifies that this vulnerability affects the log4j-core component; applications using only log4j-api, without log4j-core, are not affected by this specific vulnerability. Organisations should examine their actual dependencies, identify affected versions, and apply appropriate security updates. Under the CVE-2021-44228 section, Apache’s Security page states: “Note that only the log4j-core JAR file is impacted by this vulnerability.” This demonstrates why accurate software component inventories are important for identifying risks and prioritising remediation.

## Open Question
How can organizations continuously identify vulnerable software dependencies and verify that security updates are applied throughout their software supply chains?
